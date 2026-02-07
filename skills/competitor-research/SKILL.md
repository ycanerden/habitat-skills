---
name: competitor-research
version: 1.0.0
description: "Research competitors, map the competitive landscape, find feature gaps, and identify positioning angles. Use when the user mentions 'competitor research,' 'competitive analysis,' 'who are my competitors,' 'market landscape,' 'competitor comparison,' 'alternative analysis,' or 'how do I differentiate.' For idea-level validation, see idea-validation. For building comparison pages, see landing-page."
---

# Competitor Research

You are helping a founder understand their competitive landscape — not to copy competitors, but to find gaps, positioning angles, and opportunities they're missing.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Use the idea description, audience, and any known competitors as your starting point.

If no context exists, gather:
- What are you building? (one sentence)
- Who is it for?
- Who do you consider competitors? (even rough guesses)

## Research Process

### Step 1: Identify the Full Landscape

Don't just look at direct competitors. Map three layers:

| Type | Definition | Example |
|------|-----------|---------|
| **Direct competitors** | Same problem, same solution approach | Notion vs. Coda |
| **Indirect competitors** | Same problem, different solution approach | Notion vs. pen-and-paper |
| **Adjacent players** | Different problem, but same audience — could expand into your space | Slack adding project management |

**Research methods:**
- Search for "[problem] tool," "[problem] app," "[problem] software"
- Search for "[competitor name] alternatives" on Google
- Check Product Hunt, G2, Capterra for category listings
- Look at Reddit, Twitter/X, and relevant communities for what people recommend
- Search for "[category] market map" or "[category] landscape"

**Output:** A list of 5-15 competitors with one-line descriptions.

### Step 2: Deep-Dive on Top Competitors

For the top 3-5 direct competitors, analyze:

**Product:**
- What do they offer? (core features)
- What's their UX like? (sign up and explore if free tier exists)
- What's missing? (check their feature request forums, support threads, negative reviews)
- What's their tech stack? (check job postings, BuiltWith, Wappalyzer)

**Positioning:**
- What's their headline/tagline?
- Who do they target? (read their landing page, case studies, ads)
- What's their key differentiator?
- What tone/brand voice do they use?

**Business model:**
- Pricing tiers and price points
- Free tier or trial?
- Who's their ideal paying customer?
- Revenue signals (employee count on LinkedIn, funding raised, customer logos)

**Traction:**
- Estimated user base (check social followers, review counts, community size)
- Growth signals (hiring, funding rounds, press coverage)
- Customer sentiment (reviews on G2, Capterra, Product Hunt, Reddit)

### Step 3: Find the Gaps

This is the most important step. Look for:

**Underserved segments:**
- Who do competitors ignore? (too small, too niche, wrong geography)
- What use case is poorly served?
- What customer segment is frustrated with existing options?

**Feature gaps:**
- What do users complain about in reviews?
- What feature requests keep appearing in forums and support channels?
- What's "good enough" but not great?

**Positioning gaps:**
- Is everyone positioning the same way? (all "enterprise," all "simple," all "AI-powered")
- Is there a messaging angle no one owns?
- Is there a price point no one occupies?

**Experience gaps:**
- Where is onboarding painful?
- Where do users churn? (check negative reviews for patterns)
- What's unnecessarily complex?

### Step 4: Map Your Position

Based on the research, identify:

**Your angle:** The specific intersection of [audience] + [problem] + [approach] that you own.

Use a positioning framework:

```
For [target audience]
Who [have this problem / need]
[Product name] is a [category]
That [key benefit / what it does differently]
Unlike [primary alternative]
We [key differentiator]
```

**Create a 2x2 positioning map** using the two dimensions that matter most to your audience. Examples:
- Simple ↔ Powerful
- Cheap ↔ Premium
- Individual ↔ Team
- Generic ↔ Specialized
- Self-serve ↔ High-touch

Place competitors and yourself on the map. Identify the open quadrant.

## Output Format

### Competitive Landscape Summary

```
COMPETITIVE LANDSCAPE
─────────────────────────────────────────

Your idea: [one-liner]
Category: [market category]

DIRECT COMPETITORS
1. [Name] — [one-liner] | [pricing] | [est. size/traction]
2. [Name] — [one-liner] | [pricing] | [est. size/traction]
3. [Name] — [one-liner] | [pricing] | [est. size/traction]

INDIRECT COMPETITORS
1. [Name] — [how they solve it differently]
2. [Name] — [how they solve it differently]

KEY GAPS IDENTIFIED
1. [Gap] — [why it's an opportunity]
2. [Gap] — [why it's an opportunity]
3. [Gap] — [why it's an opportunity]

YOUR POSITIONING ANGLE
[Positioning statement]

RISKIEST COMPETITIVE THREAT
[What could kill you — and how to defend against it]
```

### Competitor Detail Cards

For each top competitor, provide a card:

```
[COMPETITOR NAME]
Website: [url]
Tagline: [their headline]
Target: [who they serve]
Pricing: [tiers and price points]
Strengths: [what they do well]
Weaknesses: [where they fall short]
Key insight: [the one thing to learn from them]
```

### Positioning Map

A text-based 2x2 showing where competitors sit and where your opening is.

### Actionable Recommendations

- **Differentiation strategy:** How to position against the top 2-3 competitors
- **What to steal:** Best practices worth adopting from competitors
- **What to avoid:** Mistakes competitors are making that you can sidestep
- **Messaging angles:** 2-3 headline/positioning options based on the gaps found

## Principles

- **Research, don't assume.** Use real data — reviews, pricing pages, community posts. Don't guess.
- **Gaps over features.** The goal isn't a feature checklist. It's finding where the market is underserved.
- **Honest assessment.** If a competitor is strong, say so. Help the founder compete where they can win.
- **Actionable output.** Every insight should connect to a decision: build this, avoid that, position here.
- **Time-appropriate depth.** For a Habitat evening, a focused 30-minute competitive scan beats a 3-week deep-dive. Match the founder's stage.

## Research Tools

When researching competitors, use:
- **Web search** for finding competitors, pricing, reviews
- **WebFetch** for reading competitor websites, landing pages, feature pages
- **Company review sites** (G2, Capterra, Product Hunt) for user sentiment

## Related Skills

- `founder-context` — Set up context with known competitors
- `idea-validation` — Validate the idea in context of competition
- `landing-page` — Build a landing page that differentiates
- `mvp-scope` — Scope MVP based on competitive gaps
