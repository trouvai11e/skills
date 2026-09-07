# Language: Chinese-to-English math drafts

When the source is Chinese or strongly Chinese-influenced English, do not translate clause by clause.

## Workflow

1. Extract the mathematical content first: the claim, its hypotheses, the logical link to neighbors (cause, contrast, reduction, conclusion). Restore connectives that Chinese prose elides.
2. Rebuild each sentence around an explicit subject–verb spine; Chinese topic-comment chains do not map to English one-to-one.
3. Verify that hedging strength matches the mathematics: Chinese drafts often overstate ("completely solved") or use vague intensifiers ("very important"); mathematical English wants the exact claim.
4. Apply `language/en.md` sentence rules last.

## Common Chinese-influenced patterns to fix

- "Although ..., but ..." — English allows only one of the two. Pick one.
- "As far as ... is/are concerned" — spoken-style filler; usually delete and let the sentence start directly.
- "In order to" -> "To".
- Repeated "This paper / In this paper" sentence openings, especially in the abstract.
- Redundant "ones": "the eigenvalues of importance are those ones with negative real part" -> "the important eigenvalues are those with negative real part".
- Noun piled on noun without articles: "Let $A$ be square matrix with full rank" -> "Let $A$ be a square matrix of full rank".
- One enormous sentence with subject and verb miles apart ("In this section a new three-dimensional ... system ... is introduced") — split into two or three short sentences.
- Abbreviation inflation: defining CS, LS, DS, SC, IE to save space makes prose unreadable and invites misreading (CS = computer science, LS = least squares). Spell out unless the abbreviation is standard in the field.
- Direct carries from Chinese rhetoric: opening the introduction with universally known background ("众所周知，……在……中起着越来越重要的作用") — delete and start with the actual problem (Higham's delete-the-first-sentence test).
- Modesty or boast conventions that do not translate: no "our paper is immature" apologies; no "extremely important" self-evaluation.
- Overuse of "because/since" and "therefore/hence" on one page — vary with as, due to, it follows that, consequently, it follows from ... that (see the connective gradation in `references/math-phrasebook.md`).
