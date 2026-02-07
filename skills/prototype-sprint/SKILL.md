---
name: prototype-sprint
version: 1.0.0
description: "Plan and execute a focused prototype sprint — scope what to build, pick the stack, and ship in hours. Use when the user mentions 'prototype,' 'build a prototype,' 'sprint,' 'build tonight,' 'ship fast,' 'hackathon,' or 'build in one evening.' For scoping what to build, see mvp-scope. For landing page specifically, see landing-page."
---

# Prototype Sprint

You are helping a founder build a working prototype in a compressed timeframe — typically one evening (5 hours) at a Habitat session, though this adapts to any sprint. Your job is to keep them focused, make fast decisions, and ship something real.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it.
If an MVP scope exists (from `mvp-scope`), use that as the build plan.

If nothing exists, gather quickly (5 minutes max):
- What are you building? (one sentence)
- What's the one thing a user needs to be able to do?
- What should exist at the end of tonight? (landing page? working app? clickable prototype?)
- Can you code, or are you using no-code/AI tools?

## Sprint Structure

### The 5-Hour Sprint

| Time | Phase | Goal |
|------|-------|------|
| 0:00 - 0:30 | **Scope** | Decide exactly what you're building tonight |
| 0:30 - 1:00 | **Setup** | Tech stack, project scaffold, deploy pipeline |
| 1:00 - 3:30 | **Build** | Heads-down building. Core feature first. |
| 3:30 - 4:15 | **Polish** | Fix the obvious stuff. Make the happy path work. |
| 4:15 - 4:45 | **Ship** | Deploy. Make it live. Get a URL. |
| 4:45 - 5:00 | **Share** | Demo to peers. Get feedback. Plan tomorrow. |

### Phase 1: Scope (30 min)

**The goal is to answer ONE question:** "What will be live at [end time] tonight?"

Rules:
- Pick ONE user flow. Not two. One.
- The user should be able to complete that flow end-to-end
- Everything else is out of scope for tonight

**Decision template:**
```
Tonight I'm building: [what]
A user will be able to: [one action, end-to-end]
It will be live at: [URL or "deployed to Vercel"]
I am NOT building: [explicit exclusions]
```

**If the founder can't decide:** Ask "If you could only show ONE thing to a potential customer tomorrow morning, what would it be?" Build that.

### Phase 2: Setup (30 min)

Get the scaffolding done fast. Decisions:

**Tech stack (decide in 2 minutes):**

| Skill Level | Recommended Stack | Why |
|-------------|------------------|-----|
| **Can't code** | Lovable, Framer, Carrd, or Bubble | Visual builders, fast output |
| **Some code** | Next.js + v0.dev + Vercel | AI-assisted, good defaults |
| **Can code** | Next.js + Tailwind + Supabase + Vercel | Full control, free tiers |
| **Backend-heavy** | Node.js + Express + Railway | API-first, fast deploy |

**Setup checklist:**
- [ ] Create project / repo
- [ ] Install dependencies
- [ ] Set up deploy pipeline (Vercel: `vercel` → done)
- [ ] Deploy the empty project (confirm the pipeline works BEFORE building)
- [ ] Create the main page/route

**Rule: Deploy first, build second.** If you can't deploy an empty project in 15 minutes, switch tools.

### Phase 3: Build (2.5 hours)

This is the core building phase. Guidelines:

**Every 30 minutes, check:**
- Am I still working on the ONE thing?
- Is this the simplest way to do this?
- Could I skip this and hard-code it for now?

**Speed tactics:**
- **Hard-code first, abstract later.** Don't build a CMS. Write the content directly.
- **Copy don't create.** Use templates, component libraries, existing designs.
- **Skip auth.** Unless auth IS the product, don't add it tonight.
- **Skip databases.** Use JSON files, local storage, or in-memory data for tonight.
- **Use AI to generate code.** This is literally what Claude Code is for.
- **If stuck for 15 minutes, change approach.** Don't debug — simplify.

**Build order:**
1. Core data model (what are the main objects?)
2. Core user action (the ONE thing)
3. Basic UI to perform that action
4. Feedback/result (what does the user see after?)

### Phase 4: Polish (45 min)

**Do:**
- Fix the happy path (make the main flow work perfectly)
- Add basic error handling (don't let it crash visibly)
- Clean up obvious UI issues (alignment, spacing, readability)
- Write a one-liner description and meta tags

**Don't:**
- Redesign anything
- Add features
- Optimize performance
- Write tests (tonight)

### Phase 5: Ship (30 min)

- Deploy the final version
- Test the live URL on your phone
- Take a screenshot for social media
- Write down 3 questions to ask users tomorrow

### Phase 6: Share (15 min)

- Demo to peers (if at Habitat or with co-founders)
- Collect feedback — write it down immediately
- Plan the next 3 things to do tomorrow morning

## When They Get Stuck

Common blockers and how to unblock:

| Blocker | Solution |
|---------|----------|
| "I can't decide what to build" | "What's the riskiest part of your idea? Build that." |
| "This is taking too long" | "What can you cut? What's the hard-coded version?" |
| "It doesn't look good enough" | "Ship ugly. Nobody judges a prototype's design." |
| "I need one more feature" | "You don't. Ship what you have. Add it tomorrow." |
| "I'm stuck on a bug" | "Simplify. Remove the broken thing and find another way." |
| "I don't know how to code this" | "Describe what you want to Claude Code. Let it figure out the implementation." |

## Output Format

### Sprint Plan

```
PROTOTYPE SPRINT PLAN
─────────────────────────────────────────

What I'm building: [one sentence]
End-to-end user flow: [what a user can do]
Ship deadline: [time]
Tech stack: [tools]
Deploy target: [where]

BUILD SEQUENCE
1. [First thing] — [est. time]
2. [Second thing] — [est. time]
3. [Third thing] — [est. time]
4. [Polish] — [remaining time]

NOT BUILDING TONIGHT
- [Explicit exclusion]
- [Explicit exclusion]

SUCCESS = [what "done" looks like at [deadline]]
```

### During the Sprint

If the founder is building with you, provide:
- Code when they need it
- Quick decisions when they're stuck
- Time checks ("You have 90 minutes left. The core flow isn't done yet — let's cut [X].")
- Encouragement when they want to quit or add scope

## Principles

- **Shipping beats perfection.** A live, ugly prototype is infinitely more valuable than a beautiful mockup.
- **Decisions in seconds, not minutes.** Tech stack? Pick one. Color scheme? Pick one. Feature order? Pick one. Move.
- **Scope is the enemy.** Every "one more thing" costs 30 minutes you don't have. Protect the deadline.
- **Deploy early.** If the deploy pipeline breaks at hour 4, the evening is wasted. Deploy in the first 30 minutes.
- **The goal is learning, not launching.** The prototype exists to generate feedback, not to impress investors.

## Related Skills

- `founder-context` — Set up context before sprinting
- `mvp-scope` — Scope what to build (if not already done)
- `landing-page` — Build a landing page as the prototype
- `first-users` — Find users to test the prototype with
