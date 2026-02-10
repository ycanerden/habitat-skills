# Habitat Skills — Your AI Co-Founder

Steve Blank, Marc Andreessen, and Paul Graham in your pocket. An AI agent framework that gives you expert advice on fundraising, marketing, launch strategy, and growth—like having a co-founder who's done it before.

Built for [Claude Code](https://docs.anthropic.com/en/docs/claude-code) and compatible AI agents.

From the team behind [Habitat](https://joinhabitat.eu) — where 101+ founders have launched prototypes in a single evening.

## 🆕 What's New

**Autonomous Research:** Skills now use Firecrawl to autonomously research competitors, scrape pricing, and analyze positioning—no manual context required.

**Simple Mode:** Non-technical founders get copy-paste templates, guided questions, and jargon-free outputs. Just say "use simple mode" to activate.

**Demo-Ready:** Built for Friday's accelerator presentation with a complete demo flow, sample project, and backup materials.

## The "Founder as Director" Philosophy

Inspired by the methodologies of Corey Haines and the Habitat 5-hour sprint, these skills are designed to empower you to act as a **Director**. Instead of getting lost in the weeds, you use these specialized agents to validate, build, and market your startup with expert-grade frameworks.

## Available Skills

### Meta & Operations

| Skill | Description |
|-------|-------------|
| [`sprint-coach`](skills/sprint-coach/SKILL.md) | **NEW.** Your timed facilitator for a 5-hour launch sprint. Momentum over perfection. |
| [`onboarding`](skills/onboarding/SKILL.md) | Start here. Introduces Habitat Skills and sets up your environment. |

### Phase 1: Ideation & Validation
*Skills for deep research and strategic positioning.*

| Skill | Description |
|-------|-------------|
| [`founder-context`](skills/founder-context/SKILL.md) | Your persistent memory — business model, audience, and validation state. |
| [`idea-validation`](skills/idea-validation/SKILL.md) | Structured frameworks (TAM, Problem-Solution, Mom Test). |
| [`vc-research`](skills/vc-research/SKILL.md) | **NEW.** Pre-loaded insights from YC, a16z, Sequoia, Antler. Like having Horowitz, Steve Blank, or Paul Graham in your pocket. |
| [`competitor-research`](skills/competitor-research/SKILL.md) | Find gaps and identify "unfair" positioning angles. |
| [`portfolio-research`](skills/portfolio-research/SKILL.md) | **NEW.** Autonomous competitor research using Firecrawl web scraping. |
| [`customer-segments`](skills/customer-segments/SKILL.md) | Personas, pain points, and specific outreach playbooks. |

### Phase 2: Prototyping & Building
*Skills for shipping functional cores, not just code.*

| Skill | Description |
|-------|-------------|
| [`landing-page`](skills/landing-page/SKILL.md) | Conversion-focused copy and code using psychological triggers. |
| [`prototype-sprint`](skills/prototype-sprint/SKILL.md) | Execution plan for a focused build session. |
| [`mvp-scope`](skills/mvp-scope/SKILL.md) | Ruthlessly cut features down to a true, shippable MVP. |

### Phase 3: Launch & Traction
*Expert-grade marketing skills for the first 100 users.*

| Skill | Description |
|-------|-------------|
| [`social-content`](skills/social-content/SKILL.md) | **ENHANCED.** Content using PAS, AIDA, and BAB copywriting frameworks. |
| [`first-users`](skills/first-users/SKILL.md) | Find your first 10-100 users with targeted outreach playbooks. |
| [`launch-plan`](skills/launch-plan/SKILL.md) | Phased launch strategy: Pre-launch -> Launch Day -> Post-launch. |
| [`pitch-deck`](skills/pitch-deck/SKILL.md) | Elevator pitches, demo scripts, and objection prep. |

## Installation

### Quick Install (Recommended)

```bash
# Clone into your project
git clone https://github.com/ycanerden/habitat-skills.git .claude/skills/habitat
```

### Manual Install

1. Download the `skills/` folder
2. Copy it to `.claude/skills/habitat/` in your project
3. Skills will be available automatically

### Git Submodule

```bash
git submodule add https://github.com/ycanerden/habitat-skills.git .claude/skills/habitat
```

## Usage

Skills activate automatically when you ask relevant questions:

```
"Help me validate my startup idea"          → idea-validation
"Research my competitors"                    → competitor-research
"Build me a landing page"                   → landing-page
"What should my MVP include?"               → mvp-scope
"How do I find my first users?"             → first-users
```

Or invoke directly:

```
/idea-validation
/competitor-research
/landing-page
```

## Quick Start

1. Install the skills
2. Say **"Get started"** — the onboarding skill walks you through everything in under 2 minutes
3. Follow the recommended next step based on your stage

## Built by Habitat

These skills were born from 23+ prototypes launched at [Habitat](https://joinhabitat.eu) evenings — where founders go from idea to shipped product in 5 hours.

Want to build alongside 50+ others? [Join the next evening →](https://joinhabitat.eu)

## Contributing

We welcome contributions. See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Contributors
- **Can Erden** ([@ycanerden](https://github.com/ycanerden))
- **Gemini** & **Claude Code** 

### Adding a new skill
1. Create a folder in `skills/` with a `SKILL.md` file
2. Follow the format of existing skills (YAML frontmatter + markdown)
3. Keep files under 500 lines
4. Submit a PR

## License

MIT — use these however you want.
