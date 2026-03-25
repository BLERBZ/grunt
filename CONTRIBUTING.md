# Contributing to Grunt

Thank you for your interest in eliminating human grunt work.

## How to Contribute

### 1. Add an Agent Persona Template

The fastest way to contribute is to add an agent persona template to `agents/`. Each template should include:

- **Persona** — Who is this agent? What is their role?
- **Capabilities** — What grunt work do they eliminate?
- **Score baseline** — Initial effectiveness estimate (0.0–1.0)
- **Grunt units** — What tasks does this persona automate per cycle?

Use the template in `agents/TEMPLATE.md` as a starting point.

### 2. Improve the Scoring Framework

The scientific scoring framework lives in `docs/SCORING.md`. Contributions that improve measurement precision are especially welcome.

### 3. Report Grunt Work Patterns

Found a category of human grunt work that Grunt doesn't yet address? Open an issue describing:
- The grunt work pattern
- How often humans encounter it
- What an ideal agent persona would look like

## Code of Conduct

Be excellent to each other. Grunt is for everyone.

## Development Setup

```bash
git clone https://github.com/blerbz/grunt
cd grunt
grunt work
```

## Questions?

Open an issue or start a Discussion on GitHub.
