---
name: gtm-strategy
version: 1.0.0
description: "Build a go-to-market strategy — ICP definition, GTM motion selection, channel prioritization, messaging framework, and 90-day plan. Use when the user mentions 'go-to-market,' 'GTM,' 'how to reach customers,' 'sales strategy,' 'marketing strategy,' 'who should I target,' 'what channels,' 'how to grow,' 'distribution,' or 'acquisition strategy.' For finding first users manually, see first-users. For cold outreach sequences, see sales-outreach."
---

# GTM Strategy

You are helping a founder build a go-to-market strategy — a concrete plan to reach, convince, and convert their ideal customers. GTM is not a one-time document; it's a set of bets that you run, measure, and update.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Pull the target audience, problem, solution, and any existing traction.

If no context, gather:
- What's the product? (one sentence)
- Who is the target customer?
- What's the core problem you solve?
- Do you have any paying customers? How did you get them?
- What's the price point (or what are you thinking)?
- What's your runway / timeline to traction?

---

## Step 1: Define Your ICP (Ideal Customer Profile)

An ICP is not a persona — it's a description of the customer type most likely to buy fast, pay well, and refer others.

### ICP Worksheet

Work through these dimensions:

**Firmographic (B2B) or Demographic (B2C):**
- B2B: Company size, industry, geography, tech stack, funding stage, team size
- B2C: Age range, income level, lifestyle, life stage, geography

**Psychographic:**
- What does this person care about at work / in life?
- What are they measured on? What are their KPIs?
- What keeps them up at night?
- What do they read, watch, follow?

**Behavioral:**
- How do they currently solve the problem you address?
- What triggers them to look for a new solution? (the "buying moment")
- How do they evaluate and buy? (self-serve vs. sales, quick vs. long cycle)
- What makes them stick with a product once they try it?

**Deal-breakers (who is NOT your ICP):**
- Which customer types churn fastest?
- Who complains most but pays least?
- Who is expensive to serve relative to revenue?

### ICP Output Template
```
ICP: [Name it — e.g., "Bootstrapped SaaS Founders"]

WHO THEY ARE
Company/context: [describe]
Decision maker: [title/role]
Team size / budget: [range]

WHAT DRIVES THEM
Primary goal: [what they're trying to achieve]
Pain we solve: [specific pain point]
Buying trigger: [what makes them look for a solution right now]

HOW THEY BUY
Process: [self-serve / demo / committee / etc.]
Time to close: [days/weeks/months]
Budget authority: [who signs]

GREEN FLAGS (strong ICP fit)
- [Signal 1]
- [Signal 2]

RED FLAGS (not a good fit)
- [Signal 1]
- [Signal 2]
```

---

## Step 2: Choose Your GTM Motion

| Motion | Best When | Examples |
|--------|-----------|----------|
| **Product-Led (PLG)** | Low friction product, self-serve value, viral loop possible | Notion, Figma, Loom |
| **Sales-Led (SLG)** | High ACV, complex buying process, enterprise | Salesforce, Rippling |
| **Community-Led (CLG)** | Product serves a passionate community, network effects | Figma plugins, Webflow |
| **Content-Led (CLUG)** | Long buying cycles, education-heavy category | HubSpot, Intercom |
| **Outbound-Led** | Know exactly who to target, sales-driven, B2B | Most B2B SaaS at early stage |

**For most early-stage Habitat founders:** Start outbound (manual, high-touch) to learn what works, then layer in PLG or content once you understand the customer.

### Motion selection guide:
- ACV < €500/year → PLG or content first
- ACV €500–5,000/year → Outbound + self-serve trial
- ACV > €5,000/year → Sales-led, white-glove onboarding
- Community product → Community-led from day one

---

## Step 3: Score and Prioritize Channels

Rate each channel 1–3 on four dimensions:

| Channel | Reach | ICP Fit | Cost | Speed | **Total** |
|---------|-------|---------|------|-------|-----------|
| Cold email | 3 | ? | 3 | 3 | |
| LinkedIn outbound | 2 | ? | 3 | 2 | |
| Content / SEO | 3 | ? | 2 | 1 | |
| Community (Reddit, Slack) | 2 | ? | 3 | 2 | |
| Paid ads | 3 | ? | 1 | 3 | |
| Partnerships | 2 | ? | 2 | 1 | |
| Events / Habitat | 1 | ? | 2 | 2 | |
| Product Hunt / Show HN | 3 | ? | 3 | 2 | |
| Warm intros / referrals | 1 | 3 | 3 | 2 | |

Fill in ICP Fit based on where your ICP actually spends time. **Pick 2 channels max to start.** Spreading across 5 channels is how founders get traction nowhere.

---

## Step 4: Build Your Messaging Framework

Good messaging = right message × right audience × right moment.

### One-liner formula:
```
[Product] helps [ICP] [achieve outcome] without [common obstacle].
```

### Full messaging map (one per ICP segment):

**Problem statement** (their words, not yours):
→ What do they say when describing this problem to a colleague?

**Before state** (life without your product):
→ Specific, painful, time-costing situation

**After state** (life with your product):
→ Concrete, measurable outcome

**Proof points** (evidence it works):
→ Customer quote, data point, before/after metric

**Primary CTA:**
→ One action, low friction ("Start free," "Book a 20-min demo," "Join the waitlist")

### Channel-specific message adaptation:

| Channel | Tone | Length | Hook type |
|---------|------|--------|-----------|
| Cold email | Direct, respectful | 4–6 sentences | Problem hook |
| LinkedIn post | Personal, story-driven | 150–300 words | Story hook |
| Landing page | Benefit-led | Above fold: 15 words | Outcome hook |
| Reddit/Slack | Helpful, non-salesy | As needed | Value hook |
| Paid ad | Punchy | 5–15 words | Pain/curiosity hook |

---

## Step 5: 30/60/90 Day GTM Plan

### Days 1–30: Learn
**Goal:** 5–10 conversations with real ICPs. Learn what messaging lands.

- [ ] Define ICP (above)
- [ ] Build a list of 100 ICP targets
- [ ] Write 3 outreach message variants
- [ ] Book and run 10 discovery calls
- [ ] Identify the 2 strongest value props from conversations
- [ ] Close 1–3 design partners (free or heavily discounted)

**Success metric:** 10 conversations, 1–3 active users giving feedback

### Days 31–60: Test
**Goal:** Find 1 repeatable acquisition channel.

- [ ] Run A/B on outreach messaging (variant A vs. B)
- [ ] Identify which channel gets highest reply rate
- [ ] Turn top customer quotes into landing page copy
- [ ] Attempt to close first 3 paying customers
- [ ] Document the "buying path" of every person who converted

**Success metric:** 3 paying customers, clear signal on which channel works

### Days 61–90: Scale
**Goal:** Double down on what worked.

- [ ] Put 80% of effort into the winning channel
- [ ] Build a referral ask into the product/onboarding
- [ ] Set up basic CRM (even a spreadsheet works)
- [ ] Write 2–3 pieces of content around the core pain (SEO / LinkedIn)
- [ ] Aim for 10 paying customers or 100 active free users

**Success metric:** 10 paying customers, MoM growth rate > 20%

---

## Output Format

```
GTM STRATEGY
─────────────────────────────────────────

Product: [name]
Stage: [pre-launch / post-launch / growth]

ICP
─────────────────────
[ICP summary — who they are, what they need, how they buy]

GTM MOTION
─────────────────────
Primary: [motion type]
Rationale: [why this fits]

TOP 2 CHANNELS
─────────────────────
Channel 1: [name]
  Why: [reasoning]
  Tactic: [specific approach]
  Metric: [how to measure]

Channel 2: [name]
  Why: [reasoning]
  Tactic: [specific approach]
  Metric: [how to measure]

MESSAGING
─────────────────────
One-liner: [sentence]
Problem: [their words]
Before: [painful state]
After: [desirable outcome]
Proof: [evidence]
CTA: [primary action]

90-DAY PLAN
─────────────────────
Days 1–30: [focus + key tasks]
Days 31–60: [focus + key tasks]
Days 61–90: [focus + key tasks]

SUCCESS METRICS
─────────────────────
Day 30: [metric]
Day 60: [metric]
Day 90: [metric]
```

---

## Principles

- **Don't market to everyone.** The riches are in the niches. One ICP done well beats three ICP done poorly.
- **Channels are a hypothesis.** Run them like experiments. Kill channels that don't convert in 30 days.
- **Messaging comes from customers, not you.** Use their exact words. The best landing page copy comes from discovery calls.
- **Early GTM is manual.** Automate nothing until you have a repeatable motion. Manual teaches you what to automate.
- **Revenue is the scoreboard.** Not signups, not pageviews. Someone handing over money.

## Related Skills

- `mom-test` — Gather ICP insights through discovery conversations
- `customer-segments` — Define segments before picking an ICP
- `sales-outreach` — Execute the outbound channel with cold sequences
- `follow-up-tracks` — Handle leads after initial outreach
- `first-users` — Get the first 10 users before scaling GTM
- `launch-plan` — Coordinate the public launch alongside GTM
