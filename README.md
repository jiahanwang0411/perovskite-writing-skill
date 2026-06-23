# Perovskite Writing Skill / 钙钛矿论文写作技能

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](#license)

**AI-powered writing assistant for perovskite solar cell research papers.**
**AI 驱动的钙钛矿太阳能电池论文写作助手。**

Write and polish PSC manuscripts in the style of Nature Energy, Nature Communications, Science, ACS Energy Letters, and Advanced Materials — works with Codex, Claude Code, Kimi Work, QoderWork, and more.

以 Nature Energy、Nature Communications、Science、ACS Energy Letters 和 Advanced Materials 的语言风格撰写和润色钙钛矿光伏论文 — 兼容 Codex、Claude Code、Kimi Work、QoderWork 等多种 AI 工具。

---

## Why this skill / 为什么需要这个技能

This skill was **extracted from extensive close reading of recent high-impact PSC papers** published in Nature Energy, Science, Advanced Materials, ACS Energy Letters, and Nature Communications. It captures the specific syntactic patterns, rhetorical moves, and domain vocabulary that distinguish top-tier perovskite manuscripts from generic academic writing.

本技能**从精读大量近期发表于 Nature Energy、Science、Advanced Materials、ACS Energy Letters 和 Nature Communications 的高影响力钙钛矿论文**中提炼而来，捕捉了顶刊论文特有的句法模式、修辞策略和专业词汇。

Without this skill, AI tools produce grammatically correct but stylistically generic text. With it, the output matches the tone, structure, and conventions that reviewers at top journals expect.

没有这个技能，AI 工具只能产出语法正确但风格平庸的文本。有了它，输出将匹配顶刊审稿人所期望的语气、结构和学术规范。

### Before vs. After / 对比示例

| Section / 章节 | Generic AI output / 通用 AI 输出 | With this skill / 使用本技能后 |
|---|---|---|
| **Abstract opening** | "Perovskite solar cells are promising for renewable energy." | "Metal halide perovskite solar cells combine high power density with low-cost manufacturing, but durability under repeated extreme temperature cycling remains insufficiently understood." |
| **Gap statement** | "However, stability is still a problem." | "Despite progress in efficiency, the long-term operational stability under real-world outdoor conditions remains underexplored, representing a significant knowledge gap for commercialization." |
| **Results** | "The efficiency improved to 27%." | "The champion device achieved a PCE of 27.2% (certified as 26.9%, NREL), while the control retained only 24.1%, corresponding to a relative improvement of 12.9%." |
| **Mechanism** | "This is because the interface is better." | "We attribute the enhanced performance to the passivation of undercoordinated Pb²⁺ sites by the SAM monolayer, which suppresses non-radiative recombination and thereby facilitates hole extraction." |
| **Conclusion** | "In conclusion, we made a good solar cell." | "In summary, we demonstrate that dynamic regulation using photoswitchable isomeric compounds marks an advancement towards the practical application of perovskite PVs in real-world scenarios." |

---

## What it does / 功能介绍

This skill teaches AI agents to write perovskite solar cell papers following 10 core principles extracted from close reading of high-impact PSC publications:

本技能教会 AI 代理按照从高影响力钙钛矿论文提炼出的 10 项核心原则撰写论文：

1. **Funnel structure / 漏斗结构** — broad context → specific findings / 从宏观背景到具体发现
2. **Quantitative precision / 定量精确** — numbers + units + conditions for every claim / 每个结论都有数据、单位和条件
3. **Balanced confidence / 张弛有度** — hedge mechanisms, confident about data / 机理谨慎，数据自信
4. **Systematic comparison / 系统对比** — always compare to control / 始终与对照组比较
5. **Multi-technique validation / 多技术验证** — corroborate with independent methods / 用独立方法交叉验证
6. **Protocol compliance / 协议规范** — name ISOS, IEC explicitly / 明确引用标准测试协议
7. **Causal chains / 因果链** — "X induces Y, leading to Z" / "X 诱导 Y，进而导致 Z"
8. **Novelty signals / 创新信号** — "underexplored," "knowledge gap" / "尚未充分探索"、"知识空白"
9. **Impact framing / 影响框架** — molecular → device → commercialization / 分子 → 器件 → 商业化
10. **Forward-looking closure / 前瞻收尾** — end with broader implications / 以更广泛的意义收尾

---

## Supported Platforms / 支持平台

| Platform / 平台 | File / 文件 | How to use / 使用方法 |
|---|---|---|
| **OpenAI Codex** | `AGENTS.md` | Place in project root; Codex reads it automatically / 放在项目根目录，Codex 自动读取 |
| **Claude Code** | `CLAUDE.md` | Place in project root; Claude reads it on startup / 放在项目根目录，Claude 启动时读取 |
| **QoderWork** | `SKILL.md` | Install as skill via QoderWork Skills panel / 通过 QoderWork 技能面板安装 |
| **Kimi Work / ChatGPT / Gemini** | `PROMPT.md` | Copy into custom instructions or system prompt / 复制到自定义指令或系统提示词中 |

All files share the same core writing principles, adapted to each platform's instruction format.

所有文件共享同一套核心写作原则，仅针对各平台的指令格式做了适配。

---

## Files / 文件说明

| File / 文件 | Description / 描述 |
|---|---|
| `SKILL.md` | QoderWork skill definition with YAML frontmatter / QoderWork 技能定义（含 YAML 元数据） |
| `CLAUDE.md` | Claude Code project instructions / Claude Code 项目指令文件 |
| `AGENTS.md` | OpenAI Codex agent instructions / OpenAI Codex 代理指令文件 |
| `PROMPT.md` | Universal system prompt for any AI tool / 通用系统提示词，适用于任意 AI 工具 |
| `sentence-patterns.md` | 80+ sentence templates organized by section / 80+ 按章节分类的句型模板 |
| `vocabulary.md` | PSC domain vocabulary and elevated register terms / 钙钛矿领域专业词汇和高级表达 |

---

## Installation / 安装方法

### OpenAI Codex
```bash
# Copy AGENTS.md and reference files to your project root
# 将 AGENTS.md 及引用文件复制到项目根目录
cp AGENTS.md sentence-patterns.md vocabulary.md /path/to/your-project/
```

### Claude Code
```bash
# Copy CLAUDE.md and reference files to your project root
# 将 CLAUDE.md 及引用文件复制到项目根目录
cp CLAUDE.md sentence-patterns.md vocabulary.md /path/to/your-project/
```

### QoderWork
```bash
# Copy to QoderWork skills directory
# 复制到 QoderWork 技能目录
mkdir -p ~/.qoderworkcn/skills/perovskite-writing/
cp SKILL.md sentence-patterns.md vocabulary.md ~/.qoderworkcn/skills/perovskite-writing/
```

### Kimi Work / ChatGPT / Other AI Tools
Open `PROMPT.md`, copy the system prompt text, and paste it into your AI tool's custom instruction field.

打开 `PROMPT.md`，复制系统提示词文本，粘贴到你的 AI 工具的自定义指令中。

---

## Example Prompts / 使用示例

- "Write an Abstract for my perovskite tandem solar cell paper"
  "为我的钙钛矿叠层太阳能电池论文写一段摘要"

- "Rewrite this Introduction paragraph in Nature Energy style"
  "以 Nature Energy 的风格重写这段引言"

- "Polish the Results section — add quantitative comparisons and protocol references"
  "润色结果部分 — 添加定量对比和测试协议引用"

- "Generate a Conclusion with forward-looking impact statements"
  "生成一段具有前瞻性影响声明的结论"

---

## Core Content Preview / 核心内容预览

### Abstract Template / 摘要模板
```
Context (broad PSC importance)
  → Problem (specific challenge)
    → "Here we report..."
      → Mechanism (how it works)
        → Key results (PCE, retention %)
          → Broader impact (commercialization)
```

### Gap Phrases / 空白声明
- "Despite progress, X remains underexplored"
- "has received limited attention in..."
- "represents a significant knowledge gap"

### Hedging vs. Confidence / 谨慎 vs. 自信
| Context / 语境 | Tone / 语气 | Examples / 示例 |
|---|---|---|
| Mechanism / 机理 | Cautious / 谨慎 | "may originate from," "might stem from" |
| Results / 结果 | Confident / 自信 | "We demonstrate," "conclusively demonstrate" |

---

## License / 许可

MIT
