---
name: math-polishing
description: Polish, restructure, or translate English mathematical papers (research articles, surveys, computational/applied math papers) while preserving mathematical meaning, theorem hypotheses, notation, and logical rigor. Use for titles, front matter (byline, date, keywords, Mathematics Subject Classification), abstracts, introductions, main body (theorems, lemmas, proofs, numerical-result sections), conclusions, acknowledgments, reference lists, and appendices of math manuscripts, including Chinese-to-English math drafts, proofreading, and pre-submission revision. Covers math-specific wording discipline: minimal notation, proof language, theorem/lemma economy, display-equation and equation-numbering hygiene, active-voice preference, article (a/the) usage tied to mathematical uniqueness, connective choice, and a field-vocabulary/symbol glossary (math terms, symbol read-aloud forms, context-dependent notation pitfalls). Also covers revision passes (删减字句、突出重点、美容结构、善用图表) and plagiarism avoidance. Trigger on 数学论文润色、数学英文写作、数学学术论文、数学论文修改、证明润色、定理证明、英文数学写作、数学摘要、数学引言、数学文章结构、数学关键词、MSC 分类号、数学署名、数学附录、LaTeX 数学论文、math paper polishing, proof writing, theorem statement, math keywords, MSC classification.
---

# Mathematical Academic Paper Polishing — Router

This skill is split into two layers:

- A **static layer** under `static/` that holds versioned, reusable content fragments (core principles, paper-type playbooks, per-section guidance, language-specific rules).
- A **dynamic layer** (this file plus `manifest.yaml`) that detects the request's axes and loads only the fragments needed for the current job.

Do not try to apply the polishing logic from memory or from this router. Always load fragments from disk as described below.

The guidance distilled here comes from the craft of mathematical writing (Halmos, Higham, Krantz) and from a Chinese-authored handbook on writing mathematics in English. It is corpus-derived writing guidance, not any journal's official policy; obey the target journal's current author guide when they differ.

## Routing protocol

Follow these five steps every time the skill is invoked.

### 1. Load the manifest and the core layer

Read [manifest.yaml](manifest.yaml). It declares the axes (`paper_type`, `section`, `language`), the allowed values, and the file paths each value maps to.

Also read every file listed under `always_load`. These hold the default stance, failure-mode diagnosis, and output format that apply to every polish job.

### 2. Detect the axis values for this request

For each axis in the manifest, decide the value using the manifest's `detect:` hint and the user's input:

- `paper_type` — theoretical / computational / survey. Default: theoretical.
  Computational covers numerical, applied, and modeling papers with numerical
  experiments or algorithms.
- `section` — title / front-matter / abstract / intro / body / conclusion / acknowledgments /
  references / appendix. May be multiple. Ask the user if it is ambiguous and matters for
  the polish. `body` covers everything between Introduction and Conclusions,
  including theorems, proofs, and numerical-result sections. `front-matter` covers
  byline, affiliations, date, keywords, and the MSC line.
- `language` — en or zh-to-en. Detect from the draft itself.

State the detected axis values in one short line to the user before proceeding, so they can correct you cheaply. This is a progress update, not an approval gate; continue unless a necessary decision remains unresolved.

### 3. Load the matching fragments

For each axis value, Read the file mapped in the manifest. Skip the `section` axis only if the user has supplied free-floating prose with no section context.

Do **not** read every fragment in `static/`. Load only what step 2 selected.

### 4. Polish using the loaded material

Apply the loaded fragments in this priority order, matching the rule from `core/failure-modes.md`:

`paper type -> section job -> focus/structure -> theorem & proof discipline -> display & notation hygiene -> sentence polish`

1. Paper-type playbook (architecture, expected parts).
2. Section-specific job and failure modes.
3. Language-specific sentence and paragraph rules.
4. Core stance and ethics throughout.

Never change the mathematics: theorem hypotheses, quantifiers, conditions, inequalities, convergence orders, and notation must survive the polish exactly. If a sentence's mathematical meaning is ambiguous, ask or flag it — do not guess.

If a paragraph's structural problem cannot be fixed without inventing content (a missing motivation, an unjustified claim, a theorem whose hypotheses are unclear), flag it instead of papering over it.

### 5. Reach for references only when needed

The files under `references/` are deep references, not defaults. Open them on demand per the `references.on_demand` table in the manifest:

- `references/worked-examples.md` — when the user asks for an example, a rule needs a concrete demonstration, or a section is drafted from scratch: curated published exemplars and revision before/after pairs. Adapt the pattern; never copy the wording into the user's draft.
- `references/math-phrasebook.md` — when the user needs sentence patterns, proof-opening/closing formulas, connective choices, transition sentences, figure/table reporting phrases, or modifier families (noun/adjective/adverb); also when a Chinese author's draft needs idiomatic replacements.
- `references/math-vocabulary.md` — when the user needs the English term for a Chinese math term, needs to write out a symbol in words at its first definition, or must check context-dependent notation (e.g., $A > 0$ meaning positive definite vs. positive matrix).
- `references/revision-playbook.md` — when the job is a whole-manuscript pre-submission revision rather than a passage polish: deletion pass, focus check, structural cosmetics (headings, equation numbering), figure/table audit, the final checklist, and plagiarism avoidance.

When the job is a whole manuscript rather than a passage, run the consistency sweep from `core/stance.md` (notation, terminology, abbreviation, and Figure/Fig. consistency) before sentence-level work, and repeat it until a pass finds nothing new.

## Why this split

- The static layer is versioned and reviewable. Adding a new paper type or section rule is one new file plus one manifest line.
- The dynamic layer keeps each invocation cheap: only the fragments relevant to this draft enter context.
- The router itself is short on purpose. Update fragments, not this file, when adding scope.
