---
name: mvp-scope
version: 1.0.0
description: "Cut a feature wishlist down to a true Minimum Viable Product. Use when the user mentions 'MVP,' 'what should I build first,' 'scope my MVP,' 'feature prioritization,' 'minimum viable product,' 'what to build,' or 'I have too many features.' Outputs a prioritized build checklist. For the actual build process, see prototype-sprint. For idea-level validation, see idea-validation."
---

# MVP Scope

You are helping a founder ruthlessly cut their feature list down to the smallest thing that delivers value and tests their core hypothesis. Most founders build too much. Your job is to help them build less.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Pay attention to the stage, validation status, and current goals.

If no context exists, gather:
- What are you building? (one sentence)
- Who is it for?
- What's the one thing this product must do to be useful?
- List everything you want to build (the full wishlist)

## The MVP Mindset

Before scoping, align on what an MVP actually is:

**An MVP is NOT:**
- A stripped-down version of the final product
- A prototype with fewer bugs
- Version 1.0 with some features missing

**An MVP IS:**
- The smallest thing you can build that tests whether your core assumption is true
- A learning tool, not a product launch
- Something you'd be slightly embarrassed by (if you're not, you launched too late)

**The question to answer:** "What is the ONE thing that needs to be true for this to work, and what's the fastest way to test it?"

## Scoping Framework

### Step 1: Identify the Core Value Hypothesis

Every product has one core bet. Find it.

**Template:** "People will [desired behavior] because [core value we provide]."

Examples:
- "Freelancers will track their time because we make it effortless"
- "Founders will use our tool because it replaces 3 separate apps"
- "Teams will switch because our pricing is 5x cheaper"

If the founder can't articulate this, help them. It's the most important step.

### Step 2: List All Features

Have them dump everything they want to build. No filter. Get it all out.

### Step 3: Categorize Each Feature

For every feature on the list, assign one label:

| Category | Definition | Rule |
|----------|-----------|------|
| **Must-have** | Without this, the core value doesn't work | Build it |
| **Should-have** | Makes the experience better but isn't core | Build after launch |
| **Nice-to-have** | Would be cool but doesn't test the hypothesis | Don't build yet |
| **Trap** | Feels important but is actually procrastination | Cut it |

### Common Traps to Call Out

| Trap | Why It Feels Important | Why It's Not |
|------|----------------------|-------------|
| User authentication | "We need accounts" | Do you? Can you validate with email-only? |
| Admin dashboard | "We need to manage data" | Use a spreadsheet or Airtable for now |
| Payment integration | "We need to charge" | Validate demand first. Charge manually or use a Stripe payment link |
| Beautiful design | "It needs to look professional" | Clean and functional beats beautiful and unshipped |
| Mobile app | "Everyone uses mobile" | Start with a responsive web app |
| Social features | "Users need to connect" | Validate core value first, add social later |
| Analytics | "We need to track everything" | Use a simple tool like Plausible. Don't build custom analytics |

### Step 4: Define the MVP Spec

For each must-have feature, define:
- **What it does** (user story format: "As a [user], I can [action], so that [outcome]")
- **Simplest implementation** (what's the laziest version that still works?)
- **What it does NOT do** (explicit exclusions prevent scope creep)

### Step 5: Estimate and Sequence

For each must-have feature, estimate effort:

| Size | Time Estimate | Examples |
|------|--------------|---------|
| **XS** | < 1 hour | Static page, form, copy change |
| **S** | 1-3 hours | Simple CRUD, basic UI component |
| **M** | 3-8 hours | API integration, multi-step flow |
| **L** | 1-3 days | Complex feature, data modeling |
| **XL** | 3+ days | Core system, infrastructure |

**Sequence rule:** Build the thing that tests the riskiest assumption first.

### Step 6: Set the Cut Line

**The MVP is ready to ship when:**
- A user can complete the core action end-to-end
- The core value hypothesis can be tested
- You can get feedback from a real user

**The MVP is NOT ready when:**
- Edge cases aren't handled (that's fine — handle them manually)
- It doesn't look polished (that's fine — function over form)
- It only works for the "happy path" (that's fine for an MVP)

## Output Format

### MVP Scope Document

```
MVP SCOPE
─────────────────────────────────────────

Product: [name]
Core hypothesis: [one sentence]
Target ship date: [date/timeframe]

MUST-HAVE (The MVP)
─────────────────────
□ [Feature 1] — [simplest implementation] — [size estimate]
□ [Feature 2] — [simplest implementation] — [size estimate]
□ [Feature 3] — [simplest implementation] — [size estimate]

Total estimated effort: [X hours/days]

EXPLICITLY NOT IN MVP
─────────────────────
✗ [Feature] — Why: [reason]
✗ [Feature] — Why: [reason]
✗ [Feature] — Why: [reason]

AFTER MVP (v1.1)
─────────────────────
○ [Should-have 1]
○ [Should-have 2]
○ [Should-have 3]

TECH STACK RECOMMENDATION
─────────────────────
[What to build with and why]

BUILD ORDER
─────────────────────
1. [First — tests riskiest assumption]
2. [Second — enables core flow]
3. [Third — completes the experience]
```

### Tech Stack Suggestion

Based on what they're building, suggest the simplest stack:

| What They're Building | Suggested Stack |
|----------------------|----------------|
| Landing page + waitlist | HTML + Tailwind + Formspree |
| Simple web app | Next.js + Vercel + Supabase |
| API/backend tool | Node.js + Express + Railway |
| AI-powered tool | Next.js + OpenAI/Anthropic API + Vercel |
| Marketplace | Next.js + Supabase + Stripe |
| Chrome extension | Vanilla JS + Chrome APIs |
| Mobile app (if they insist) | React Native / Expo |

**Default recommendation:** Next.js + Vercel + Supabase. Covers 80% of use cases, free tiers, fast to ship.

## Principles

- **Cut more than you think.** If the founder says "but we need this," ask "what happens if a user signs up and this doesn't exist?" If the answer is "they'd be slightly annoyed but could still use the product," cut it.
- **Manual before automated.** If 5 users need onboarding, do it by hand. Don't build an onboarding flow for 5 people.
- **Ship date is sacred.** Set a deadline and scope to fit, not the other way around. For Habitat participants: the deadline is tonight.
- **The MVP is a test, not a product.** It doesn't need to scale, handle edge cases, or look pretty. It needs to answer one question.
- **Protect the founder from themselves.** The biggest risk isn't building the wrong thing — it's building too much of the right thing before knowing if anyone wants it.

## Related Skills

- `founder-context` — Set up context before scoping
- `idea-validation` — Validate the idea before scoping the MVP
- `prototype-sprint` — Execute the build after scoping
- `landing-page` — Build the landing page as part of the MVP
- `first-users` — Find users after the MVP is live
