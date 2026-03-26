# Grunt

> An ultra-intelligent, daily-generational, self-evolving system for eliminating human grunt work.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Startup: grunt work](https://img.shields.io/badge/startup-grunt%20work-brightgreen)](grunt)

---

## What is Grunt?

Grunt is an open source platform that collects, ingests, wires, and integrates **agent persona/profile templates** using a scientific method that self-iterates toward near-perfection for eliminating units of human grunt work.

Each day, Grunt:
1. Researches the internet to grow its definition of human grunt work
2. Curates and scores agent persona templates against a scientific framework
3. Self-iterates — the weakest templates are refined, the strongest are promoted
4. Reports progress on the key metric: **units of grunt work eliminated per cycle**

---

## Quick Start

```bash
# Start Grunt
grunt work
```

---

## Architecture

```
grunt/
├── agents/                        # Agent persona/profile templates
│   ├── TEMPLATE.md                # Template schema
│   ├── standup-summarizer.md      # ⭐ Gold (0.81)
│   ├── code-reviewer.md           # ⭐ Gold (0.82)
│   ├── release-notes-writer.md    # ⭐ Gold (0.83)
│   ├── pr-description-writer.md   # ✅ Pass (0.77)
│   ├── documentation-updater.md   # ✅ Pass (0.72)
│   └── grunt-ceo/                 # Grunt CEO agent (Paperclip)
├── docs/                          # Scientific method, scoring, roadmap
│   ├── VISION.md
│   ├── SCORING.md
│   └── ROADMAP.md
├── scripts/                       # Daily evolution scripts (v0.2)
└── grunt                          # Startup command (grunt work)
```

### Daily Generation Cycle

```
Internet Research → Grunt Work Identification → Agent Persona Scoring
       ↓                      ↓                         ↓
  Trend Ingestion     Task Taxonomy Update      Template Refinement
                                                         ↓
                                               Self-Iteration Report
```

---

## Agent Persona Templates

Grunt templates live in `agents/`. Each template defines:
- **Persona** — name, role, capabilities, tone
- **Score** — effectiveness rating (0.0–1.0) against the scientific framework
- **Lineage** — parent templates, iteration history
- **Grunt Units** — units of human grunt work this persona eliminates per cycle

### Template Leaderboard

| Template | Version | Composite | Tier | Grunt Work Eliminated |
|----------|---------|-----------|------|-----------------------|
| Release Notes Writer | v2 | **0.83** | ⭐ Gold | Changelog & release notes from git history |
| Code Reviewer | v2 | **0.82** | ⭐ Gold | Automated PR review for bugs, style, security |
| Standup Summarizer | v1 | **0.81** | ⭐ Gold | Async standup digests — no meetings needed |
| PR Description Writer | v1 | **0.77** | ✅ Pass | PR descriptions from diffs & commit history |
| Documentation Updater | v1 | **0.72** | ✅ Pass | Keeps docs in sync with code changes |

> **Scoring tiers:** ⭐ Gold (≥ 0.80) • ✅ Pass (0.60–0.79) • ⚠️ Review (0.40–0.59) • ❌ Fail (< 0.40)

---

## Scientific Scoring Framework

Grunt uses a multi-dimensional scoring framework to measure effectiveness:

| Dimension | Weight | Description |
|-----------|--------|-------------|
| Grunt Units Eliminated | 40% | Tasks completed per cycle |
| Autonomy Rate | 25% | Tasks completed without human intervention |
| Error Rate | 20% | Inverse of errors per 100 tasks |
| Iteration Delta | 15% | Improvement vs. prior generation |

See `docs/SCORING.md` for full specification.

---

## Roadmap

| Milestone | Target | Status |
|-----------|--------|--------|
| v0.1 — Foundation | Q2 2026 | 🚧 In Progress |
| v0.2 — Daily Cycle | Q3 2026 | Planned |
| v0.3 — Community Templates | Q4 2026 | Planned |
| v1.0 — Self-Evolving Production | 2027 | Vision |

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) and [docs/](docs/).

---

## License

MIT — see [LICENSE](LICENSE).
