# Habitat Skills — AI Agent Skills for Founders

A collection of AI agent skills that help aspiring founders go from idea to launched product. Built for [Claude Code](https://docs.anthropic.com/en/docs/claude-code) and compatible AI coding agents.

From the team behind [Habitat](https://joinhabitat.eu) — where 101+ founders have launched prototypes in a single evening.

## What are skills?

Skills are markdown files that give AI agents specialized knowledge. Install them in your project, and your agent knows how to validate ideas, research competitors, scope MVPs, and build landing pages — using the same frameworks experienced founders use.

## Available Skills

### Phase 1: Ideation & Validation

| Skill | Description |
|-------|-------------|
| [`founder-context`](skills/founder-context/SKILL.md) | Set up your project context so all other skills know your idea, audience, and stage |
| [`idea-validation`](skills/idea-validation/SKILL.md) | Validate your idea with structured frameworks — TAM, problem-solution fit, Mom Test |
| [`competitor-research`](skills/competitor-research/SKILL.md) | Research competitors, find gaps, and identify positioning angles |
| [`customer-segments`](skills/customer-segments/SKILL.md) | Generate customer segments with personas, pain points, and outreach per segment |

### Phase 2: Prototyping & Building

| Skill | Description |
|-------|-------------|
| [`landing-page`](skills/landing-page/SKILL.md) | Build a conversion-focused landing page — copy, structure, and code |
| [`prototype-sprint`](skills/prototype-sprint/SKILL.md) | Plan and execute a focused prototype sprint — scope, prioritize, build |
| [`mvp-scope`](skills/mvp-scope/SKILL.md) | Cut your feature list down to a true MVP with a clear build checklist |

### Phase 3: Demo & Pitch

| Skill | Description |
|-------|-------------|
| [`pitch-deck`](skills/pitch-deck/SKILL.md) | Create pitches — 30-second elevator pitch, demo scripts, objection prep |

### Phase 4: Launch & Traction

| Skill | Description |
|-------|-------------|
| [`first-users`](skills/first-users/SKILL.md) | Find your first 10, then 100 users with a targeted outreach playbook |
| [`launch-plan`](skills/launch-plan/SKILL.md) | Create a phased launch strategy — pre-launch, launch day, post-launch |
| [`social-content`](skills/social-content/SKILL.md) | Create launch posts, build-in-public updates, and social media content |

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
2. Run `/founder-context` to set up your project context
3. Start building — try `/idea-validation` to test your idea

## Built by Habitat

These skills were born from 23+ prototypes launched at [Habitat](https://joinhabitat.eu) evenings — where founders go from idea to shipped product in 5 hours.

Want to build alongside 50+ others? [Join the next evening →](https://joinhabitat.eu)

## Contributing

We welcome contributions. See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Adding a new skill

1. Create a folder in `skills/` with a `SKILL.md` file
2. Follow the format of existing skills (YAML frontmatter + markdown)
3. Keep files under 500 lines
4. Submit a PR

## License

MIT — use these however you want.
