# Claude Code Skills Marketplace

A curated collection of high-quality skills for [Claude Code](https://claude.ai/claude-code).

Skills extend Claude Code with specialized capabilities — domain expertise, analysis pipelines, design systems, and workflow automation. Install any skill with a single command.

## Install a Skill

```bash
# Clone directly into Claude Code's skills directory
git clone <github-url> ~/.claude/skills/<skill-name>

# Or clone anywhere and symlink
git clone <github-url> ~/my-skills/<skill-name>
ln -sf ~/my-skills/<skill-name> ~/.claude/skills/<skill-name>
```

Restart Claude Code after installing. The skill will appear in the available skills list and trigger automatically based on context.

### Update a Skill

```bash
cd ~/.claude/skills/<skill-name> && git pull
```

## Available Skills

### Health & Biomedical

| Skill | Description | Methods | Install |
|-------|-------------|---------|---------|
| [**Apple Health Deep Analysis**](https://github.com/labrinyang/apple-health-analysis) | Mayo Clinic-grade health data analysis for Apple Health exports. 20 peer-reviewed statistical methods, 35+ SVG visualizations, clinical-quality HTML reports. | Granger Causality, Transfer Entropy, CCM, Sample Entropy, DFA, LBGI/HBGI, Cosinor, Bayesian Change Points, Biological Age | `git clone https://github.com/labrinyang/apple-health-analysis ~/.claude/skills/apple-health-analysis` |

---

## What Makes a Good Skill?

| Criteria | Description |
|----------|-------------|
| **Depth over breadth** | A skill should do one thing exceptionally well, not many things adequately |
| **Evidence-based** | Cite papers, use validated methods, reference clinical guidelines |
| **Graceful degradation** | Handle missing data, edge cases, and errors without crashing |
| **Self-contained** | Zero external dependencies — Python stdlib only for scripts |
| **Multi-language** | Support at least English; bonus for Chinese, Spanish, etc. |
| **Visual output** | Generate HTML reports, charts, or visualizations where appropriate |
| **Tested** | Include eval test cases with assertions |

## Submit a Skill

Want to add your skill to the marketplace? Open a PR with:

1. Add your skill to the appropriate category table in this README
2. Ensure your skill repo has:
   - `SKILL.md` with proper frontmatter (name, description)
   - `README.md` with installation instructions
   - `LICENSE` (MIT recommended)
   - Test cases in `evals/`
3. Your skill should follow the quality criteria above

## Categories

We organize skills into these domains. If your skill doesn't fit, propose a new category in your PR.

- **Health & Biomedical** — Health data analysis, medical knowledge, bioinformatics
- **Data Science** — Statistical analysis, visualization, ML pipelines
- **Software Engineering** — Code review, testing, deployment, architecture
- **Design** — UI/UX, visual design, design systems
- **DevOps & Infrastructure** — CI/CD, monitoring, cloud deployment
- **Research & Writing** — Paper analysis, documentation, technical writing
- **Productivity** — Workflow automation, project management, planning

## License

MIT — This marketplace index is open source. Individual skills have their own licenses.
