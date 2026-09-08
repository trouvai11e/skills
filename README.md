# Skills

A collection of custom skills for AI coding agents (pi, Claude Code, and other agents supporting the SKILL.md convention).

## Installation

Copy the skill folder you need into your agent's skills directory:

```bash
# pi / generic agent skills directory
cp -r math-polishing ~/.agents/skills/

# Claude Code
cp -r math-polishing ~/.claude/skills/
```

Restart the session; the agent will load the skill automatically when its trigger words match.

## Skills

| Skill | Description | Example triggers |
|---|---|---|
| [math-polishing](math-polishing/) | English polishing for mathematical academic papers: polishes titles, front matter (byline, keywords, MSC), abstracts, introductions, main body (theorems/proofs/numerical results), conclusions, acknowledgments, references, and appendices while preserving mathematical meaning (theorem hypotheses, quantifiers, convergence orders, notation) exactly; includes a math vocabulary/symbol glossary, a whole-manuscript revision playbook, and plagiarism-avoidance rules | math paper polishing, proof writing, theorem statement, 数学论文润色 |

## Structure convention

Each skill follows a static/dynamic split:

```
skill-name/
├── SKILL.md          # Router: axis detection and loading protocol
├── manifest.yaml     # Declares axes and fragment paths
├── static/           # Core stance + per-axis rule fragments
│   ├── core/
│   └── fragments/
└── references/       # On-demand deep references (phrasebooks, examples, checklists)
```

## License

[MIT](LICENSE)
