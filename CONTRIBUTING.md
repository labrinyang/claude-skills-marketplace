# Contributing to Claude Code Skills Marketplace

Thank you for your interest in contributing a skill!

## Submission Process

### 1. Build Your Skill

Your skill repo must contain:

```
your-skill/
├── SKILL.md          # Required — skill instructions with frontmatter
├── README.md         # Required — installation guide + feature description
├── LICENSE           # Required — MIT recommended
├── scripts/          # Optional — bundled analysis/generation scripts
├── references/       # Optional — domain knowledge, reference ranges
└── evals/
    └── evals.json    # Recommended — test cases for validation
```

### 2. SKILL.md Frontmatter

```yaml
---
name: your-skill-name
description: >
  What the skill does and when to trigger it.
  Be specific about trigger phrases and contexts.
---
```

### 3. Quality Checklist

Before submitting, verify:

- [ ] Skill works with `claude install-skill <your-repo-url>`
- [ ] Scripts require only Python 3.6+ stdlib (no pip dependencies)
- [ ] Missing/incomplete data is handled gracefully (no crashes)
- [ ] At least 2 test cases in `evals/evals.json`
- [ ] README includes installation command and usage examples
- [ ] No hardcoded personal data, API keys, or secrets
- [ ] Skill description is specific enough to trigger correctly

### 4. Submit a PR

1. Fork this marketplace repo
2. Add your skill to the appropriate category table in `README.md`
3. Format: `| [**Skill Name**](url) | Description | Key methods/features | Install command |`
4. Open a PR with title: `Add skill: your-skill-name`

### 5. Review Criteria

We evaluate submissions on:

| Criteria | Weight | Description |
|----------|--------|-------------|
| Utility | 30% | Does it solve a real problem people have? |
| Quality | 25% | Is the analysis/output rigorous and accurate? |
| Robustness | 20% | Does it handle edge cases and missing data? |
| Design | 15% | Is the output well-formatted and visually clear? |
| Documentation | 10% | Is the README clear? Are methods cited? |

## Skill Categories

Add your skill to the category that best fits. Current categories:

- **Health & Biomedical**
- **Data Science**
- **Software Engineering**
- **Design**
- **DevOps & Infrastructure**
- **Research & Writing**
- **Productivity**

If none fit, propose a new category in your PR description.
