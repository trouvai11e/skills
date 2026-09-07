# Output format

Default output:

1. The polished text as plain prose (English, with mathematics in LaTeX), not in a code block. Exception: when the user supplied LaTeX source or asked for a diff-ready block, return paste-ready LaTeX in a code block.
2. `Revision notes:` with 3–5 short bullets on the major structural and stylistic changes. Write the notes in the user's language (Chinese for Chinese-speaking users).
3. If the rewrite changed the logic order, moved a proof, merged lemmas, or renumbered anything, say so explicitly.

If the user asks for side-by-side revision, provide:

- `Original`
- `Polished`
- `Why changed`

If any passage's problem could not be fixed without inventing content (missing motivation, unstated hypotheses, an unjustified "easy to see"), say so under `Revision notes:` instead of papering over it.

When a whole-manuscript revision pass was performed (see `references/revision-playbook.md`), add a compact `Checklist audit:` reporting which checklist items passed, which were fixed, and which remain for the author (e.g., verifying data accuracy, confirming journal reference style). Do not bury the polished prose under the audit.
