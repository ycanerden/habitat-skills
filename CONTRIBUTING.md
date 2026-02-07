# Contributing to Habitat Skills

Thanks for wanting to contribute. Here's how.

## Adding a New Skill

1. Create a folder in `skills/` with your skill name (lowercase, hyphens only)
2. Add a `SKILL.md` file with YAML frontmatter:

```yaml
---
name: your-skill-name
version: 1.0.0
description: "When to use this skill. Include trigger phrases for discoverability."
---
```

3. Write the skill content following these conventions:
   - Keep it under 500 lines
   - Use H2/H3 headings and bullet points
   - Include a "Before Starting" section that checks for `founder-context.md`
   - Include an "Output Format" section
   - Include a "Principles" section
   - Include a "Related Skills" section
   - Be opinionated — tell founders what to do, not just what they could do

4. Add a `references/` subfolder for any supporting reference files

5. Update `AGENTS.md` to include your skill in the registry

6. Submit a PR with:
   - What the skill does
   - Why it's useful for founders
   - Example usage

## Improving an Existing Skill

- Fix errors, add examples, improve frameworks
- Keep changes focused — one improvement per PR
- Explain what you changed and why in the PR description

## Skill Quality Guidelines

**Good skills are:**
- Actionable (tell founders what to do, not just what to think about)
- Opinionated (make recommendations, don't just list options)
- Stage-aware (adapt to whether someone has 5 hours or 5 weeks)
- Honest (don't promise miracles, acknowledge trade-offs)
- Connected (reference related skills for natural workflows)

**Avoid:**
- Generic advice ("do customer research")
- Overly academic frameworks without practical application
- Skills that duplicate existing ones
- Content over 500 lines (split into skill + references)

## Code of Conduct

Be helpful, be honest, be kind. We're building tools for founders who are putting themselves out there. Let's make it easier for them.
