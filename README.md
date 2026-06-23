# Perovskite Writing Skill

An AI agent skill for writing and polishing **perovskite solar cell research papers** in the style of top-tier journals (Nature Energy, Nature Communications, Science, ACS Energy Letters, Advanced Materials).

## What it does

This skill teaches AI agents to write PSC manuscripts following 10 core principles extracted from close reading of high-impact perovskite papers:

- **Funnel structure** — every section moves from broad context to specific findings
- **Quantitative precision** — all claims backed by numbers with units and conditions
- **Balanced confidence** — hedge in mechanism, confident in empirical results
- **Multi-technique validation** — results corroborated by independent methods
- **Causal chain construction** — explain mechanisms through cause-effect sequences
- **Novelty signaling** — consistent gap vocabulary
- **Impact framing** — molecular innovation → device metrics → commercialization potential

## Files

| File | Description |
|------|-------------|
| `SKILL.md` | Core skill definition — writing principles, section templates, usage instructions |
| `sentence-patterns.md` | 80+ ready-to-use sentence patterns organized by paper section |
| `vocabulary.md` | Domain-specific vocabulary and phrasing for PSC research |

## How to use

### With QoderWork

1. Open QoderWork
2. Go to Skills > Install Skill
3. Import the `.skill` file or copy the files to `~/.qoderworkcn/skills/perovskite-writing/`
4. In any conversation, ask the AI to write or polish a perovskite paper section

### Example prompts

- "Write an Abstract for my perovskite tandem solar cell paper"
- "Rewrite this Introduction paragraph in Nature Energy style"
- "Polish the Results section — add quantitative comparisons and protocol references"

## Supported sections

Abstract, Introduction, Results & Discussion, Conclusion, and Experimental Methods.

## License

MIT
