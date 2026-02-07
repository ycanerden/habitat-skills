---
name: customer-segments
version: 1.0.0
description: "Generate and analyze customer segments — personas, job titles, pain points, where to find them, and personalized outreach per segment. Use when the user mentions 'customer segments,' 'target audience,' 'customer persona,' 'who are my customers,' 'ICP,' 'ideal customer profile,' 'buyer persona,' 'customer discovery,' or 'who should I sell to.' For outreach execution, see first-users. For idea-level validation, see idea-validation."
---

# Customer Segments

You are helping a founder identify, prioritize, and reach their best customer segments. The goal is to move from "everyone could use this" to "these 3 specific groups need this most, and here's exactly how to reach them."

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Use the idea, target audience, and validation info as your starting point.

If no context exists, gather:
- What are you building? (one sentence)
- What problem does it solve?
- Who do you think the customer is? (even a rough guess)
- Is this B2B, B2C, or both?

## Segmentation Framework

### Step 1: Generate Initial Segments

Create 3-5 distinct customer segments. For each segment:

**Segment profile:**

| Field | Description |
|-------|-------------|
| **Segment name** | 2-4 words that describe the group (e.g., "Solo Freelance Designers") |
| **Company type** | Industry + size (e.g., "Design agencies, 5-20 employees") |
| **Job titles** | 2-3 specific roles (e.g., "Freelance UI Designer, Design Lead, Creative Director") |
| **Pain intensity** | How badly they need this (Critical / High / Moderate) |
| **Why they'd care** | One sentence — the specific value prop for THIS segment |
| **Current solution** | How they solve this today (competitor, manual process, nothing) |
| **Willingness to pay** | Estimated (High / Medium / Low) with reasoning |
| **Where to find them** | 2-3 specific channels (communities, platforms, events) |

### Step 2: Prioritize Segments

Not all segments are equal. Rank them using this matrix:

| Factor | Weight | Questions |
|--------|--------|-----------|
| **Pain intensity** | High | How urgent is the problem? Are they actively searching for solutions? |
| **Reachability** | High | Can you actually get in front of them? Do you have access to their channels? |
| **Willingness to pay** | Medium | Will they pay for this? Do they have budget authority? |
| **Segment size** | Medium | Is this segment large enough to build a business? |
| **Ease of serving** | Low | How complex is it to deliver value to them? |

**Scoring:**
- Rate each segment 1-5 on each factor
- Multiply by weight (High = 3x, Medium = 2x, Low = 1x)
- Total score determines priority

**Output:** Rank segments from highest to lowest priority. Recommend focusing on the top 1-2 segments first.

### Step 3: Deep-Dive on Top Segments

For the #1 priority segment, create a detailed profile:

**Demographics:**
- Company size, industry, geography
- Typical revenue range
- Team structure

**Psychographics:**
- What do they value? (speed, quality, cost savings, status)
- What frustrates them about current solutions?
- How do they make buying decisions? (individual, team, committee)
- What language do they use to describe the problem?

**Behavioral:**
- Where do they spend time online? (specific subreddits, Slack groups, LinkedIn groups, newsletters)
- What do they search for? (Google queries, keywords)
- What events do they attend?
- Who do they follow / trust? (influencers, thought leaders, publications)

**Buying journey:**
- How do they discover new tools? (search, recommendations, ads, communities)
- Who makes the purchase decision?
- What would trigger them to switch from their current solution?
- What objections would they have?

### Step 4: LinkedIn Search Queries

For each segment, generate a short LinkedIn search query that would find these specific people:

**Format:** `"[job title]" AND "[industry keyword]" AND "[company size indicator]"`

**Examples:**
- `"Freelance Designer" AND "UI" AND "remote"`
- `"Head of Marketing" AND "SaaS" AND "Series A"`
- `"Founder" AND "e-commerce" AND "Shopify"`

Provide 2-3 variations per segment to maximize coverage.

### Step 5: Personalized Outreach Per Segment

For each segment, create a tailored outreach message. The message should:
- Reference the specific pain point THIS segment faces
- Use the language THIS segment uses
- Offer value relevant to THIS segment's situation
- End with a low-friction ask

**DM / Email template per segment:**

```
Hi [name],

I noticed you [specific observation about them — their role, company, or something they posted].

Quick question: [problem question specific to their segment]?

I'm building [product] — it [one sentence, framed for THIS segment's pain point].

Would you be open to a 10-minute chat? I'd love to understand how you handle [specific task] today.

[your name]
```

**Provide 2-3 message variants per segment:**
- Variant A: Direct (lead with the problem)
- Variant B: Curiosity (lead with a question)
- Variant C: Value-first (lead with a useful insight or resource)

## Output Format

### Customer Segments Overview

```
CUSTOMER SEGMENTS
─────────────────────────────────────────

Product: [name]
Problem: [one sentence]

SEGMENT 1: [Name] ⭐ TOP PRIORITY
────────────────────
Company type: [industry + size]
Job titles: [2-3 roles]
Pain intensity: [Critical/High/Moderate]
Why they'd care: [one sentence]
Current solution: [what they do today]
Willingness to pay: [High/Medium/Low]
Where to find them: [2-3 channels]
LinkedIn search: "[query]"
Priority score: [X/50]

SEGMENT 2: [Name]
────────────────────
[same format]

SEGMENT 3: [Name]
────────────────────
[same format]

RECOMMENDED FOCUS
────────────────────
Start with Segment [X] because [reason].
Test with [N] people from [specific channel].
If they respond well, expand to Segment [Y].
```

### Detailed Profile (Top Segment)

```
DEEP DIVE: [Segment Name]
─────────────────────────────────────────

DEMOGRAPHICS
[Details]

PSYCHOGRAPHICS
[Details]

BEHAVIORAL
[Details]

BUYING JOURNEY
[Details]

OUTREACH MESSAGES
────────────────────
Variant A (Direct):
[Message]

Variant B (Curiosity):
[Message]

Variant C (Value-first):
[Message]

LINKEDIN SEARCHES
────────────────────
1. [Query]
2. [Query]
3. [Query]
```

## Principles

- **Specific beats broad.** "Solo freelance designers who use Figma and have 3-10 clients" is useful. "Designers" is not.
- **Pain intensity is the #1 filter.** The segment with the most urgent pain will respond fastest, pay most, and give the best feedback.
- **Real language matters.** Use words your segment uses. If they say "finding clients," don't write "customer acquisition."
- **Start with one segment.** Trying to reach 5 segments at once means reaching none well. Pick one, validate, expand.
- **Segments can be wrong.** The point isn't to get it perfect — it's to have a hypothesis to test. Outreach will tell you if you're right.
- **B2B tip:** The user (who uses the product) and the buyer (who pays) are often different people. Map both.

## Related Skills

- `founder-context` — Set up context before segmentation
- `idea-validation` — Validate whether the segment has the problem
- `first-users` — Execute outreach to the segments you've identified
- `competitor-research` — Understand what alternatives each segment uses
- `landing-page` — Tailor landing page messaging to the top segment
