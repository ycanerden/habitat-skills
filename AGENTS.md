# Habitat Skills — Agent Configuration

This repository contains AI agent skills for founders building startups from scratch. Skills provide structured frameworks for ideation, validation, prototyping, and launch.

## Skill Registry

Each skill is a markdown file at `skills/<skill-name>/SKILL.md` with YAML frontmatter.

### Available Skills

- `onboarding` — First-time user experience. Introduces skills, shows immediate value, sets up context progressively
- `founder-context` — Deep-dive context enrichment (business model, team, validation) that all other skills reference
- `idea-validation` — Validate startup ideas using structured frameworks
- `competitor-research` — Research competitors, map gaps, find positioning angles
- `customer-segments` — Generate customer segments with personas, pain points, and outreach per segment
- `landing-page` — Build conversion-focused landing pages
- `prototype-sprint` — Plan and execute focused prototype sprints
- `mvp-scope` — Scope a true MVP from a feature wishlist
- `pitch-deck` — Create pitches — 30-second elevator pitch, demo scripts, objection prep
- `first-users` — Find first 10-100 users with targeted playbooks
- `launch-plan` — Create phased launch strategies
- `social-content` — Create launch posts, build-in-public updates, and social media content

## Skill Format

### Required

- `name`: 1-64 chars, lowercase a-z, numbers, hyphens. Must match directory name.
- `description`: 1-1024 chars. Describe what it does and when to use it.

### Optional

- `version`: Semantic version (default: 1.0.0)
- `license`: License identifier (default: MIT)

### Structure

```
skills/
  skill-name/
    SKILL.md          # Main skill file (required)
    references/       # Supporting reference files (optional)
```

## Conventions

- Keep SKILL.md under 500 lines
- Use H2/H3 headings and bullet points for scannability
- Include trigger phrases in descriptions so agents can match intent
- Reference related skills to help agents pick the right one
- Check for `founder-context` before gathering info — avoid re-asking what's already known

## Context File

The `founder-context` skill creates `.claude/founder-context.md` in the user's project. All other skills should check for this file before asking questions.
