# Revision playbook (deep reference — whole-manuscript pass)

Load this when the job is a full pre-submission revision, not a passage polish. "All writing benefits from revision" (Higham). Method: read aloud, find what sounds wrong, diagnose, then cut and rewrite. Let the draft cool for days before revising; revise as a reader, not as the author.

## 1. Deletion pass (删减字句)

The most frequent revision act is deletion. Cut everything dispensable; what the author finds prettiest is often what most needs cutting.

- Shorten sentences; question every passive verb; prune redundant words; replace noun phrases with verbs (Dixon's rules).
- "Thus there arises the question of whether ..." -> "The question arises whether ..."
- "As a matter of fact the solution of equation (9) is an optimal solution" -> "The solution of equation (9) is actually an optimal one."
- "The eigenvalues of importance are those ones with negative real part" -> "The important eigenvalues are those with negative real part."
- "As far as a uniform bound ... is concerned it can be estimated by ..." -> "A uniform bound ... can be estimated by ..."
- "The program was found to be a suitable tool by means of which the computational experiments were performed" -> "We performed the computational experiments with the program."
- Delete repeated sentence patterns: if three lemma proofs all open "According to the definition of matrix eigenvalues, ...", keep it once.
- Do not re-derive textbook steps: "Using the Cauchy–Schwarz inequality, we obtain ..." suffices.
- Do not repeat background already detailed in the author's earlier papers; state the known results and cite.
- A statement-and-proof can often be halved by omitting well-known facts (mean-value arguments, the triangle inequality) and unused equation labels — see the Yorke-inequality example pattern: state the claim with minimal wrapper, choose the point, estimate, done.

## 2. Focus pass (突出重点)

- One theme per paper. Cut any section that does not orbit it (the algebraic-geometry history lesson in a paper about solving polynomial systems).
- Not a textbook: cite, don't reteach, the wider field's basics.
- Applications framing must not crowd out the results themselves.
- Sectioning balance: merge half-page subsections; split monoliths so novelty and difficulty are visible.
- A long paper needs a Conclusions section — the three-minute pitch test: could the author sell the paper to a colleague in three minutes from it?
- Too many theorems = no theorem. Keep the best one or two (at most three or four); merge known or similar lemmas; inline minor facts.
- Length is not merit: Nash's dissertation was a dozen pages; Chern's intrinsic Gauss–Bonnet proof was six.

## 3. Structural cosmetics (美容结构)

- Title: shorten to the load-bearing words; remove logically redundant modifiers.
- Section headings: consistent capitalization and numbering style; no equation numbers in headings; no singleton subsections (a 1.1 with no 1.2); delete words already present in the parent heading.
- Equation numbers: audit against the rule — referenced later, or the conclusion formula of a theorem/lemma. Delete the rest; add missing ones. One number per logical formula, even when displayed over two lines.
- Long single sentences with subject and verb far apart: split into two or three.
- Abbreviations: remove all but field-standard ones.
- Symbols/definitions introduced but barely used: inline or delete.
- References: reformat every entry to the target journal's style; one author-name order, one abbreviation scheme, one "and"/"&" choice, complete fields, alphabetical order for math journals; delete uncited entries; add missing key works; never hide the authors' own closely related prior paper from the list — that is a honesty problem, not a style one.

## 4. Figures and tables (善用图表)

Displays serve three purposes: verify the model/analysis on real examples, compare with existing methods (convergence rate, complexity, stability), and give readers a visual sense of the results. For theory-led papers they are supporting actors — limited space.

- Twenty-plus figures: cut toward half. One or two representative displays per phenomenon; narrate the rest.
- Captions: standard, compact, informative — not telegraphic, not paragraphs.
- Every displayed figure/table must be discussed in the text: why shown, what it proves, why it deserves the space. Undiscussed displays are deleted.
- Professional quality only: colors, line styles, labels. Poor figures antagonize referees.

## 5. Worked example pattern (condensed case study)

From the revision of "A new chaotic attractor coined":

- Title: "A new chaotic attractor connecting the Lorenz attractor and the Chen attractor" -> "A new chaotic attractor coined" (three "attractor"s removed; curiosity added).
- Abstract: mixed first/third person and referenced "system (1)" and "[1], [2]" -> third person, self-contained: "This letter reports the finding of a new chaotic attractor in a simple three-dimensional autonomous system, which connects the Lorenz attractor and the Chen attractor and represents the transition from one to the other."
- Keywords: dropped non-key items and plurals -> "Chaos; Lorenz attractor; Chen's attractor."
- Intro: "The new system is very important since it bridges the famous Lorenz system and the Chen system" -> "The new system plays the role of bridging the Lorenz system and the Chen system."
- Headings: removed a singleton Subsection 1.1, fixed capitalization, dropped "(1.1)" from a heading, unified Section-number punctuation.
- Body: one 60-word sentence with subject miles from its verb -> three short sentences. CS/LS/DS/SC/IE abbreviation thicket -> spelled out.
- A "strange function" definition used nowhere later -> inlined.
- References: unified author order, journal abbreviations, "&", page style, added missing city/author data, lowercased preprint title words.

Result: three pages, accepted in one month, referee comment "very well written".

## 6. Final checklist

Run every item; report pass/fix/author-action:

- Spelling and grammar checked (tool-assisted)?
- Title accurate, concise, proportionate?
- Abstract self-contained, informative, no "In this paper"-type filler, no symbols/formulas/bare citation numbers?
- Introduction rigorous, objective, complete? History traceable? Problem well posed? Results described factually?
- Section headings apt, balanced, smoothly connected?
- Proofs step-by-step sound? Theorem hypotheses independent and complete? Too many theorems?
- Formulas well displayed? Anything inline that should be displayed? Every equation number necessary? Any missing?
- Notation consistent throughout? Simplifiable without misleading?
- Conclusions distinct from the abstract? Looking both back and forward?
- References: right quantity, obtainable, relevant, consistent format, journal style, no uncited entries, no missing citations?
- Funding and helpful colleagues/referees acknowledged?
- Figures/tables: support the theory, data reliable, discussed in text?
- Any word/phrase/sentence deletable without changing meaning?
- Any overlong sentence? Repeated sentence patterns? Passive convertible to active?
- Sentence and paragraph order optimal?
- Copied quotations, citations, and numerical data verified against the source?
- Quoted material properly credited? All sources listed? Anyone's work under-credited?

## 7. Plagiarism avoidance (避免抄袭)

Zero tolerance in the West; consequences include failed degrees and lost jobs.

What counts as plagiarism:

- anyone else's sentences or paragraphs without quotation marks and citation;
- light paraphrase — changing a few words or reordering does not remove plagiarism; the original idea in a similar sentence is still protected;
- translating part of a foreign-language paper without attribution;
- self-plagiarism: verbatim reuse of more than a few lines from the authors' own published work (co-authors and publishers hold rights);
- bulk reuse of web/book definitions and proofs with cosmetic word swaps;
- anyone's figure — even illustrative — without permission: unpublished figures need the author's consent, published figures need the publisher's (usually free, but required), plus acknowledgment in the caption and a reference entry.

How to avoid: write in your own sentences, from your own understanding; quote with quotation marks and cite; give predecessors their due — it costs nothing. Anti-plagiarism software will find copied sentences; check before submission.
