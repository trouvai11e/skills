# math-polishing

数学学术论文英文润色 skill。在**严格保持数学含义**（定理条件、量词、收敛阶、不等号方向、记号）不变的前提下，对数学论文的各个部分进行润色、重构或中译英。

写作指导原则提炼自《数学之英文写作》及 Halmos、Higham、Krantz 的数学写作经典论述。

## 功能范围

- **按章节润色**：题目、摘要、引言、主体（定理/引理/证明、数值结果节）、结论、致谢、参考文献
- **按论文类型**：理论型、计算/应用型、综述型
- **按语言**：英文草稿润色、中文草稿/中式英语的翻译重构
- **整稿投稿前修订**：删减字句、突出重点、美容结构（标题/章节标题/公式编号）、图表审查、检查清单
- **数学英语专项**：符号最小化（"最好的符号是没有符号"）、证明用语、连词强调梯度、冠词 a/the 用法、主动语态优先、公式与文字的排版配合
- **学术规范**：避免抄袭（含自我抄袭、图表授权、引用改写边界）

## 触发词

数学论文润色、数学英文写作、数学学术论文、数学论文修改、证明润色、定理证明、英文数学写作、数学摘要、数学引言、LaTeX 数学论文、math paper polishing、proof writing、theorem statement

## 安装

```bash
# pi / 通用 agent skills 目录
cp -r math-polishing ~/.agents/skills/

# Claude Code
cp -r math-polishing ~/.claude/skills/
```

重启会话后自动生效。

## 工作原理

采用静态/动态分层路由，每次调用只加载与当前任务相关的规则碎片：

```
SKILL.md          路由器：五步路由协议
manifest.yaml     声明三个坐标轴及碎片路径
static/core/      每次必加载：立场、失败模式诊断、输出格式
static/fragments/ 按轴加载：
  paper_type/     theoretical / computational / survey
  section/        title / abstract / intro / body / conclusion /
                  acknowledgments / references
  language/       en / zh-to-en
references/       按需加载：
  math-phrasebook.md      数学英语短语库（句型、证明用语、连词、图表报告用语）
  revision-playbook.md    整稿修订手册（删减/重点/结构/图表/清单/抄袭）
  worked-examples.md      发表级范例与改前/改后对照
```

润色优先级链：

```
论文类型 → 章节职能 → 主题聚焦 → 定理证明纪律 → 公式符号卫生 → 句子润色
```

结构问题先于句子问题；无法在不虚构内容的情况下修复的段落会被明确标出，而不是用漂亮话掩盖。
