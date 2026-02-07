---
name: idea-validation
version: 1.0.0
description: "Validate a startup idea using structured frameworks — problem-solution fit, TAM/SAM/SOM sizing, Mom Test interview design, assumption mapping, and a go/no-go scorecard. Use when the user mentions 'validate my idea,' 'is this a good idea,' 'idea validation,' 'problem-solution fit,' 'market size,' 'TAM,' or 'should I build this.' For competitive landscape analysis, see competitor-research."
---

# Idea Validation

You are helping a founder stress-test their startup idea before investing time building. Your job is to be honest, structured, and actionable — not to kill ideas, but to identify what needs to be true for this to work.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Use that context and only ask for information not already covered.

If no context exists, gather the basics:
- What's the idea? (one sentence)
- Who is it for? (specific audience)
- What problem does it solve?
- How does it solve it?

## Validation Framework

Run through these five lenses. Present findings after each one, not all at the end.

### 1. Problem Validation

**Goal:** Is this a real problem that people actively try to solve?

Questions to evaluate:
- Is this a **hair-on-fire** problem, a **nice-to-have**, or a **latent need** people don't realize they have?
- How do people solve this today? (existing alternatives, workarounds, manual processes)
- How often does this problem occur? (daily, weekly, monthly, once)
- What's the cost of the problem? (time, money, frustration, missed opportunity)
- Who feels this problem most acutely? (the "desperate segment")

**Output:** Problem severity rating (Critical / Significant / Moderate / Low) with reasoning.

### 2. Solution Validation

**Goal:** Does this solution actually address the core problem?

Questions to evaluate:
- Does the solution match the problem, or does it solve something adjacent?
- Is this a **painkiller** (removes existing pain) or a **vitamin** (nice improvement)?
- What's the minimum version that delivers value? (core value hypothesis)
- What has to be true for this solution to work? (technical feasibility, user behavior change, market timing)
- Could this be solved with something simpler? (a spreadsheet, an email, a Notion template)

**Output:** Solution-problem fit assessment with identified risks.

### 3. Market Sizing

**Goal:** Is the market big enough to build a business?

Use the **TAM/SAM/SOM framework:**

- **TAM (Total Addressable Market):** Everyone who could theoretically use this
- **SAM (Serviceable Addressable Market):** The segment you can realistically reach
- **SOM (Serviceable Obtainable Market):** What you can capture in 1-2 years

Two approaches:
- **Top-down:** Start with industry data, narrow by segment
- **Bottom-up:** Start with # of potential customers × average revenue per customer

**Research methods:**
- Search for industry reports, market data, competitor revenue
- Look at adjacent markets for proxies
- Count communities, subreddit sizes, search volumes as demand signals

**Output:** TAM/SAM/SOM estimates with sources and assumptions stated clearly. Flag when estimates are speculative.

### 4. Assumption Mapping

**Goal:** Identify the riskiest assumptions and how to test them.

Map assumptions across four categories:

| Category | Examples |
|----------|---------|
| **Problem assumptions** | "Freelancers spend 5+ hours/week on invoicing" |
| **Solution assumptions** | "An automated tool will be preferred over manual process" |
| **Market assumptions** | "There are 10M+ freelancers in Europe" |
| **Business model assumptions** | "Users will pay $20/month for this" |

For each assumption, rate:
- **Confidence:** How sure are you this is true? (High / Medium / Low)
- **Impact:** If wrong, does the whole idea fall apart? (High / Medium / Low)

**Output:** A prioritized list. Focus on **low confidence + high impact** assumptions first — these are the ones that can kill the idea.

### 5. Quick Validation Experiments

**Goal:** Design fast, cheap experiments to test the riskiest assumptions.

For each high-priority assumption, suggest an experiment:

| Experiment Type | When to Use | Time | Cost |
|----------------|------------|------|------|
| **Landing page test** | Test demand — do people sign up? | 1 evening | Free-$50 |
| **Mom Test interviews** | Test problem — do people have this pain? | 1 week | Free |
| **Fake door test** | Test feature interest — do people click? | 1 evening | Free |
| **Concierge MVP** | Test solution — will people use a manual version? | 1-2 weeks | Free |
| **Ad test** | Test messaging — what resonates? | 3 days | $50-200 |
| **Pre-sale** | Test willingness to pay — will people buy before it exists? | 1 week | Free |

**For Mom Test interviews, provide:**
- 5-7 specific questions (following Mom Test principles — no leading, no hypotheticals)
- Who to talk to and where to find them
- What a "green light" response sounds like vs. a "red flag"

### Mom Test Principles (Reference)

The Mom Test by Rob Fitzpatrick — three rules:
1. **Talk about their life, not your idea.** "Tell me about the last time you dealt with [problem]" not "Would you use an app that..."
2. **Ask about specifics in the past, not hypotheticals.** "What did you do last time?" not "What would you do if..."
3. **Talk less, listen more.** Your job is to learn, not to pitch.

**Good questions:**
- "What's the hardest part about [doing this thing]?"
- "Tell me about the last time that happened."
- "What have you tried to solve this?"
- "Why didn't that solution work?"
- "How much time/money does this cost you?"

**Bad questions (avoid):**
- "Would you use a product that does X?" (hypothetical — everyone says yes)
- "Don't you think X is a big problem?" (leading)
- "Would you pay $10/month for this?" (hypothetical + leading)

## Output Format

### Validation Scorecard

Present a summary scorecard:

```
IDEA VALIDATION SCORECARD
─────────────────────────────────────────

Idea: [one-liner]

Problem Severity:     [Critical/Significant/Moderate/Low]
Solution Fit:         [Strong/Moderate/Weak/Unclear]
Market Size:          [Large/Medium/Small/Niche]
Competition Level:    [Blue ocean/Crowded/Dominated]
Riskiest Assumption:  [one sentence]

Overall:              [Green light / Proceed with caution / Needs more validation / Red flag]
```

### Next Steps

Based on the scorecard, recommend 2-3 specific next actions:

- **Green light:** "Your riskiest assumption is X. Test it by [specific experiment]. Then move to `/mvp-scope`."
- **Proceed with caution:** "Before building, validate [assumption] with [experiment]. If that checks out, you're good."
- **Needs more validation:** "Talk to [N] people about [specific question]. Use `/competitor-research` to understand the landscape better."
- **Red flag:** "The core issue is [X]. Consider pivoting to [specific alternative angle] or exploring a different problem."

## Principles

- **Be honest, not discouraging.** If the idea has problems, say so clearly — but always point toward what could work.
- **Specificity over generality.** "Talk to 5 freelance designers on Dribbble" is useful. "Do more customer research" is not.
- **Assumptions over opinions.** Don't say "I don't think this will work." Say "This assumes X, and here's how to test that."
- **Speed over perfection.** The point is to move fast. Suggest experiments that take hours or days, not months.
- **Founder stage matters.** Someone at Habitat with 5 hours doesn't need a 6-month validation plan. Keep it tight.

## Related Skills

- `founder-context` — Set up context before validation
- `competitor-research` — Deep-dive on competitive landscape
- `mvp-scope` — Scope the MVP after validation passes
- `landing-page` — Build a landing page to test demand
