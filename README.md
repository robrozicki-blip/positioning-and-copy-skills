# Positioning & Copy Skills

A Cowork plugin for Claude Code with marketing skills. Inspired by [Infinite Headcount](https://github.com/MikeFishbeinAtherial/infinite-headcount).

## Skills

### `/positioning-and-copy:competitive-positioning`
3-phase competitive intelligence and positioning workflow:
- **Phase 1** — Claude grills you on your ICP, differentiator, and what made your last clients say yes. One question at a time, with a hypothesis.
- **Phase 2** — Drop competitor URLs. Claude scrapes each site and builds full battle cards (ICP, delivery model, memorable lines, weaknesses), then a side-by-side comparison table.
- **Phase 3** — Positioning canvas grounded in your answers and real competitor data. Category name, ICP, pillars, headline options.

Output: Self-contained HTML file with dark theme and sidebar navigation.

### `/positioning-and-copy:landing-page-copy`
Full homepage copy in one pass. Hero, Problem, Features, Who It's For, Social Proof, CTA. Each section labeled.

Output: Structured JSON + readable markdown in chat.

### `/positioning-and-copy:interrogate-me`
8-question marketing intake. Run before any content, copy, or campaign work. Outputs a reusable Marketing Brief that other skills reference automatically.

## Install as a Cowork Plugin

```bash
claude plugin install --from https://github.com/robrozicki-blip/positioning-and-copy-skills
```

Or test locally:

```bash
git clone https://github.com/robrozicki-blip/positioning-and-copy-skills.git
claude --plugin-dir ./positioning-and-copy-skills
```

## Recommended Workflow

1. **`/positioning-and-copy:interrogate-me`** — Build a Marketing Brief
2. **`/positioning-and-copy:competitive-positioning`** — Deep competitor research + positioning canvas
3. **`/positioning-and-copy:landing-page-copy`** — Full homepage copy grounded in your positioning

## Structure

```
.claude-plugin/
  plugin.json            # Plugin manifest
skills/
  competitive-positioning/
    SKILL.md
  landing-page-copy/
    SKILL.md
  interrogate-me/
    SKILL.md
```
