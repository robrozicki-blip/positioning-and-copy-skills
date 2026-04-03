# Positioning & Copy Skills

Marketing skills for Claude Code. Inspired by [Infinite Headcount](https://github.com/MikeFishbeinAtherial/infinite-headcount).

## Skills

### `/competitive-positioning`
3-phase competitive intelligence and positioning workflow:
- **Phase 1** — Claude grills you on your ICP, differentiator, and what made your last clients say yes. One question at a time, with a hypothesis.
- **Phase 2** — Drop competitor URLs. Claude scrapes each site and builds full battle cards (ICP, delivery model, memorable lines, weaknesses), then a side-by-side comparison table.
- **Phase 3** — Positioning canvas grounded in your answers and real competitor data. Category name, ICP, pillars, headline options.

Output: Self-contained HTML file with dark theme and sidebar navigation.

### `/landing-page-copy`
Full homepage copy in one pass. Hero, Problem, Features, Who It's For, Social Proof, CTA. Each section labeled.

Output: Structured JSON + readable markdown in chat.

### `/interrogate-me`
8-question marketing intake. Run before any content, copy, or campaign work. Outputs a reusable Marketing Brief that other skills reference automatically.

## Setup

Clone this repo and the skills are available via Claude Code when you work inside it:

```bash
git clone https://github.com/robrozicki-blip/positioning-and-copy-skills.git
cd positioning-and-copy-skills
```

Then use `/competitive-positioning`, `/landing-page-copy`, or `/interrogate-me` in Claude Code.

## Workflow

The recommended flow:

1. **`/interrogate-me`** — Build a Marketing Brief
2. **`/competitive-positioning`** — Deep competitor research + positioning canvas
3. **`/landing-page-copy`** — Full homepage copy grounded in your positioning
