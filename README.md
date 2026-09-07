# Skills

[English](#english) | [中文](#中文)

---

## 中文

AI 编程助手（pi / Claude Code 等支持 SKILL.md 规范的 agent）可用的自定义 skill 合集。

### 安装

将需要的 skill 文件夹复制到你的 agent skills 目录：

```bash
# pi / 通用 agent skills 目录
cp -r math-polishing ~/.agents/skills/

# Claude Code
cp -r math-polishing ~/.claude/skills/
```

重启会话后，agent 会根据 skill 的触发词自动加载。

### Skill 列表

| Skill | 说明 | 触发词示例 |
|---|---|---|
| [math-polishing](math-polishing/) | 数学学术论文英文润色：保持数学含义（定理条件、量词、收敛阶、记号）不变的前提下，润色题目、摘要、引言、主体（定理/证明/数值结果）、结论、致谢与参考文献；含整稿修改流程（删减字句、突出重点、美容结构、善用图表）与避免抄袭规范 | 数学论文润色、数学英文写作、证明润色、数学摘要、LaTeX 数学论文 |

### 结构约定

每个 skill 遵循静态/动态分层：

```
skill-name/
├── SKILL.md          # 路由器：轴检测与加载协议
├── manifest.yaml     # 声明坐标轴与碎片路径
├── static/           # 核心立场 + 按轴划分的规则碎片
│   ├── core/
│   └── fragments/
└── references/       # 按需加载的深参考（短语库、范例、修订清单）
```

### 许可证

[MIT](LICENSE)

---

## English

A collection of custom skills for AI coding agents (pi, Claude Code, and other agents supporting the SKILL.md convention).

### Installation

Copy the skill folder you need into your agent's skills directory:

```bash
# pi / generic agent skills directory
cp -r math-polishing ~/.agents/skills/

# Claude Code
cp -r math-polishing ~/.claude/skills/
```

Restart the session; the agent will load the skill automatically when its trigger words match.

### Skills

| Skill | Description | Example triggers |
|---|---|---|
| [math-polishing](math-polishing/) | English polishing for mathematical academic papers: polishes titles, abstracts, introductions, main body (theorems/proofs/numerical results), conclusions, acknowledgments, and references while preserving mathematical meaning (theorem hypotheses, quantifiers, convergence orders, notation) exactly; includes a whole-manuscript revision playbook and plagiarism-avoidance rules | math paper polishing, proof writing, theorem statement |

### Structure convention

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

### License

[MIT](LICENSE)
