# Paper type: Theoretical (pure / theory-heavy)

Typical architecture:

`Preliminaries -> Main results -> Proofs (or outline of proofs) -> Extensions`

## Theorem and lemma economy

- One main theorem, two at most three or four notable results. A ten-page paper carrying ten theorems and lemmas has no center. Merge or demote the rest: fold similar lemmas into one with parts (i), (ii); state minor known facts in a line of text instead of a formal lemma.
- A lemma earns its own environment only if it is used in several places or is genuinely technical. Known results gathered for the reader's convenience should be summarized, not numbered one by one.
- Place each lemma immediately before the theorem whose proof uses it, not in a pile at the front.

## Theorem statements

- The statement must be self-contained: every hypothesis used in the proof (introduced during derivation, assumed earlier in prose) must appear in the statement. A theorem's name and conclusion are what get quoted — its conditions travel with it.
- Separate clearly what is new from what is known: put known auxiliary results in Preliminaries, labeled as such.
- In the statement of a theorem/lemma, the key formulas should carry equation numbers; in proofs, number only formulas referenced later.

## Proofs

- Long proofs get signposts: an outline sentence ("We divide the proof into four steps"), then step markers. See `references/math-phrasebook.md` for the formulas.
- For very long or highly technical proofs in papers aimed partly at applied readers, consider moving the full proof to an appendix and keeping a proof sketch near the statement. Pure math papers normally keep proof and statement together — most mathematicians will not accept a theorem they cannot read the proof of.
- Compress elementary steps: "Using the Cauchy–Schwarz inequality and the standard energy method, we obtain ..." instead of a page of routine manipulation.
- Never write "It is easy to see" or "It is trivial" unless a referee can verify it in a minute. When in doubt, give the one-line reason instead.
