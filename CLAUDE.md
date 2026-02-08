# Habitat Skills

This is a collection of AI agent skills for founders. Skills are markdown files in `skills/` that provide structured frameworks for building startups.

## Key conventions

- Every skill has a `SKILL.md` with YAML frontmatter (name, description)
- Skills should check for `.claude/founder-context.md` before gathering context
- Keep skill files under 500 lines
- Reference related skills to help with routing
- All skills follow the same pattern: gather context → apply framework → deliver actionable output

## First-time users

When a user starts a new session and no `.claude/founder-context.md` exists in their project, suggest running the onboarding skill: "Looks like this is your first time. Say **get started** and I'll walk you through Habitat Skills in under 2 minutes."

The onboarding skill shows value immediately from just one sentence, then gathers context progressively. It replaces the old approach of asking 20 questions upfront.
