# Grunt Roadmap

## v0.1 — Foundation (Q2 2026) — In Progress

**Goal**: Establish the schema, scoring framework, and template library baseline.

- [x] `grunt work` startup command
- [x] Agent persona template schema defined (`agents/TEMPLATE.md`)
- [x] Scientific scoring framework documented (`docs/SCORING.md`)
- [x] 5 agent persona templates shipped (3 Gold, 2 Pass)
- [x] GitHub repo live at github.com/BLERBZ/grunt
- [ ] Contributing guide clear enough for first external contributor
- [x] Update README with template leaderboard (current scores)
- [x] `.gitignore` committed

**Template Leaderboard (v0.1):**

| Template | Version | Composite | Tier |
|----------|---------|-----------|------|
| Release Notes Writer | v2 | 0.83 | Gold |
| Code Reviewer | v2 | 0.82 | Gold |
| Standup Summarizer | v1 | 0.81 | Gold |
| PR Description Writer | v1 | 0.77 | Pass |
| Documentation Updater | v1 | 0.72 | Pass |

## v0.2 — Automated Scoring Pipeline (Q3 2026)

**Goal**: Eliminate manual scoring. Every template change triggers automated evaluation.

**Phase 1: CI Scoring (weeks 1-3)**
- [ ] `scripts/score-template.sh` — CLI tool that parses a template file and validates score math
- [ ] GitHub Actions workflow: on PR touching `agents/*.md`, run score validation
- [ ] Reject PRs where stated composite doesn't match calculated composite
- [ ] Auto-comment on PRs with score diff vs. prior version

**Phase 2: Daily Cycle (weeks 4-6)**
- [ ] `scripts/daily-cycle.sh` — orchestrator for daily evolution
- [ ] Internet research integration — scan for new grunt work patterns (HN, Reddit, dev surveys)
- [ ] Template candidate generator — given a grunt work pattern, scaffold a v1 template
- [ ] Weekly evolution report auto-generated and committed to `reports/`

**Phase 3: Leaderboard Automation (weeks 7-8)**
- [ ] README template leaderboard auto-updates on merge to main
- [ ] Score history tracked per template (JSON in `scores/`)
- [ ] Regression detection — alert if a template's score drops between generations

## v0.3 — Community & Beta (Q4 2026)

**Goal**: Open the platform for community contributions and begin real-world validation.

**Phase 1: Contributor Infrastructure (weeks 1-4)**
- [ ] Template submission via PR workflow with automated validation
- [ ] PR template with checklist (schema compliance, score estimation, grunt work evidence)
- [ ] First-contributor onboarding: issue labels (`good-first-template`), guided template wizard
- [ ] Community Discussions enabled on GitHub

**Phase 2: Beta Program (weeks 5-8)**
- [ ] Beta tester recruitment — 10 teams using Grunt templates in real workflows
- [ ] Usage data collection — anonymized GUE measurements from beta testers
- [ ] Replace estimated scores with measured scores from real-world data
- [ ] Beta feedback loop: testers suggest improvements, maintainers iterate templates

**Phase 3: Template Marketplace (weeks 9-12)**
- [ ] Searchable, filterable template catalog (static site or GitHub Pages)
- [ ] Tags/categories: language, framework, team size, grunt work type
- [ ] "Install" flow — copy template to your project with one command

## v1.0 — Self-Evolving Production (2027)

**Goal**: Grunt improves itself. Templates evolve without human input.

**Phase 1: Self-Revision Engine**
- [ ] Given a template with score < Gold, automatically generate a v(n+1) candidate
- [ ] A/B evaluation — compare template versions against a standard task set
- [ ] Auto-promote improvements, auto-retire regressions (3 consecutive fails)

**Phase 2: Multi-Agent Tournament**
- [ ] Templates compete head-to-head on identical tasks
- [ ] Elo-style ranking system supplements the composite score
- [ ] Cross-pollination — high-scoring techniques from one template applied to others

**Phase 3: Production Infrastructure**
- [ ] Self-hosting dashboard (deploy your own Grunt instance)
- [ ] API for template discovery and scoring
- [ ] Plugin system — integrate Grunt templates into IDEs, CI/CD, Slack

---

_Last updated: 2026-03-26 by Grunt CEO_
_Owner: Grunt CEO_
