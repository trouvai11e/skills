# Section: Body (main text between Introduction and Conclusions)

Everything from the end of the introduction to the start of the conclusions. Paper-type architecture (preliminaries/results/proofs vs. problem/method/analysis/numerics) lives in the `paper_type/` fragments; this file holds the writing discipline shared by both.

## Focus

- One paper, one theme. Everything orbits it. Do not write the paper like a textbook: background belonging to the wider field gets a citation, not an exposition.
- Sectioning must be balanced: merge half-page fragments; split a monolith so that the novel and difficult parts are visible landmarks.
- Sentences and paragraphs must follow the reasoning order — logical, sequential, smooth. No jumps. Use paragraph-opening transitions ("We now turn to ...", "With the help of the preceding two lemmas we can now prove ...") — see `references/math-phrasebook.md`.

## Display-equation discipline

- No unbroken chains of five or more displayed equations/inequalities without intervening text. Let the reader breathe: split a ten-line derivation into two or three chunks with commentary between.
- Compress routine derivations: "Using the Cauchy–Schwarz inequality, the standard energy method, and the Grönwall inequality, we obtain ..." — do not spell out elementary manipulation.
- Display (own-line) any formula that is important, long, or referenced later; keep short inline math inline.

## Equation numbering

- Number a formula if and only if it is referenced later, or it is the conclusion formula inside a theorem/lemma statement. Unreferenced numbers are clutter; a thesis draft with 98 numbers where most are never cited needs a purge.
- Never repeat a displayed formula; reference its number.
- One formula split over two lines gets one number, not two.

## Proofs

- Signpost long proofs (outline sentence, step markers). Proof-opening/closing/omitting formulas are in `references/math-phrasebook.md`.
- "It is easy to see / trivial / obvious" — use only when a referee can verify immediately; otherwise supply the one-line reason. Reviewers punish unexplained "obvious".

## Symbols and definitions

- Introduce each symbol or definition at first need, not in a front-loaded dump. A definition used once ("c = 2.8", a named function never used again) should be inlined or deleted — every unnecessary symbol taxes the reader's memory.
- Check every symbol is used, defined once, and used with one meaning.

## Figures and tables

- Every figure/table must be discussed in the text: why it is shown, what it demonstrates, why it deserves the space. Undiscussed displays get cut.
- "Figure" vs. "Fig.": pick one per journal style and enforce it throughout; "Figs. 1 and 2", not "Fig. 1 and Fig. 2"; capital F.
- Keep only representative, professional-quality figures; merge similar ones; narrate the rest.
