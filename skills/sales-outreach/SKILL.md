---
name: sales-outreach
version: 1.0.0
description: "Write cold outreach sequences — email and LinkedIn — tailored to your ICP and product. Use when the user mentions 'cold email,' 'outreach,' 'cold outreach,' 'email sequence,' 'LinkedIn outreach,' 'how to reach prospects,' 'outbound,' 'sales emails,' 'prospecting,' or 'write me an email to.' For handling replies and follow-ups after first contact, see follow-up-tracks. For booking discovery calls, see mom-test."
---

# Sales Outreach

You are helping a founder write cold outreach that gets replies — not spam. Cold outreach works when it's relevant, brief, and focused on the prospect's problem, not your product.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Use the ICP, problem, and solution.

If no context, gather:
- What's the product? (one sentence)
- Who are you reaching out to? (specific role/title + context)
- What problem do they have that you solve?
- What's the ask? (demo call, trial, feedback, intro?)
- Do you have any social proof? (customers, results, traction)
- Email, LinkedIn, or both?

---

## Cold Outreach Principles

### What makes outreach work

1. **Relevance first.** They need to feel like this was written for them, not blasted to 10,000 people.
2. **One problem, one ask.** Don't list 5 features. Pick the sharpest pain point. One CTA.
3. **Short is respectful.** 4–7 sentences max. Busy people don't read walls of text.
4. **No attachments, no decks, no links.** In the first email. Earn the right to share more.
5. **The goal is a reply, not a sale.** You're opening a conversation, not closing a deal.

### The anatomy of a great cold email

```
Subject: [short, specific, personal — 4–6 words]

Opening: [1 sentence that shows you know them / their world]
Problem: [1–2 sentences on the pain they likely have]
Solution: [1 sentence on what you do — outcome-focused, not feature-focused]
Proof:   [1 sentence — customer result, traction, or credibility]
Ask:     [1 sentence — one clear, low-friction CTA]

[First name]
```

Total: under 100 words whenever possible.

---

## Email Sequence Types

### Type 1: Problem-Led (Best for cold outreach)

Lead with their pain before mentioning your product.

```
Subject: [specific pain they recognize]

Hi [Name],

[Observation about their role/company that signals you did homework — 1 sentence.]

Most [ICP type] I talk to are dealing with [specific problem] — [consequence of that problem].

[Product name] fixes that by [outcome in one phrase]. [One customer/result sentence.]

Worth a 20-minute call to see if it applies to you?

[Your name]
```

**Example:**

```
Subject: Engineering invoices eating your Fridays?

Hi Sarah,

I saw you're leading a 12-person design studio — nice work on the Volta rebrand.

Most studio owners I talk to lose 3–4 hours every Friday chasing invoices and reconciling time sheets manually.

We built Billow to handle that automatically — studios like Forma cut invoice time by 80% in their first month.

Worth a 20-minute call to see if it applies to Atelier?

Tom
```

---

### Type 2: Result-Led (Best when you have strong proof)

Lead with a result, then explain how.

```
Subject: How [similar company] [achieved result]

Hi [Name],

[Similar company] used [your product] to [specific result] in [timeframe].

They were dealing with [problem] — [product] solved it by [mechanism].

You're [similar context], so I thought this might be relevant.

Open to a quick chat?

[Your name]
```

---

### Type 3: Referral / Warm Intro (Highest reply rate)

When you have a mutual connection or can mention a recognizable name.

```
Subject: [Mutual name] suggested I reach out

Hi [Name],

[Mutual name] mentioned you might have [problem] — I hope it's okay I'm reaching out.

We help [ICP type] [solve problem] — [one result sentence].

Would you be open to a 15-minute call this week?

[Your name]
```

---

### Type 4: Feedback Ask (For very early stage, no traction yet)

Lower-stakes ask when you have no proof points.

```
Subject: Quick question from a founder

Hi [Name],

I'm building [product] for [ICP] — [one sentence on the problem].

Before I go further, I'd love 15 minutes with someone like you to make sure I'm solving the right problem.

No pitch, just questions. Would that work?

[Your name]
```

---

## LinkedIn Outreach

### Connection request note (300 char limit)

```
Hi [Name] — I noticed [specific thing about their profile/company/post].
I'm working on [brief context] and your perspective would be valuable.
Would love to connect.
```

Keep it under 200 characters. Don't pitch in the connection request.

### After connecting: First DM

Wait 1–2 days after connecting.

```
Thanks for connecting, [Name].

[One observation about their work / pain point].

We built [product] for exactly this — [one-line outcome].
Happy to share more if it's relevant to what you're working on.

No pressure either way.
```

### LinkedIn note on tone

LinkedIn messages can be slightly warmer than email. Use a conversational tone, reference something specific in their profile or recent post. Never use LinkedIn InMail templates that feel copy-pasted.

---

## Subject Line Variants

Write 3 subject line A/B variants for each campaign:

| Type | Example |
|------|---------|
| Specific pain | "Freelance invoicing taking your Sundays?" |
| Number/result | "2 hours back every week for design studios" |
| Direct / curious | "Quick question about your onboarding" |
| Name drop | "Saw your post about [topic]" |
| Mutual | "[Name] suggested I reach out" |

**Avoid:**
- "Following up on my last email" (as a subject line)
- "Quick question" (overused)
- All caps or exclamation marks
- Anything that sounds like a newsletter or marketing blast

---

## Personalization at Scale

Even when reaching out to 100 people, add at least one personalized line per email. Sources:

| Source | What to reference |
|--------|------------------|
| LinkedIn | Recent post, career change, company news |
| Company website | Product launch, team page, job postings |
| Mutual connections | Who introduced or connected you |
| Industry news | Relevant news item about their space |
| Their content | Article, podcast, talk they gave |

**Template for personalization:**
```
{{first_name}} — I noticed {{personalization_observation}}.
```

---

## Sequence Cadence (Before Handoff to Follow-Up Tracks)

This skill handles the **initial outreach only**. For follow-ups, use `follow-up-tracks`.

| Day | Action | Notes |
|-----|--------|-------|
| Day 0 | Send email 1 (primary) | Problem-led or result-led |
| Day 3 | Follow-up if no reply | See `follow-up-tracks` |
| Day 7 | Follow-up if no reply | |
| Day 14 | Final follow-up | Breakup email |

---

## Output Format

Generate ready-to-send outreach for the founder:

```
OUTREACH PACKAGE
─────────────────────────────────────────

Target: [role/ICP]
Channel: [email / LinkedIn / both]
Goal: [demo / feedback / intro / trial]

EMAIL 1 — PROBLEM-LED
─────────────────────
Subject A: [option]
Subject B: [option]
Subject C: [option]

---

Hi {{first_name}},

[Body — 5–7 sentences]

[Your name]

---

EMAIL 1 — RESULT-LED (VARIANT)
─────────────────────
Subject A: [option]
...

---

LINKEDIN CONNECTION NOTE
─────────────────────
[Under 200 chars]

LINKEDIN FIRST DM (after connecting)
─────────────────────
[3–5 sentences]

PERSONALIZATION HOOKS
─────────────────────
Things to research per prospect:
- [Hook 1]
- [Hook 2]
- [Hook 3]

REPLY HANDLING
─────────────────────
If positive → [see follow-up-tracks: warm lead track]
If no reply → [see follow-up-tracks: ghosted track]
If objection → [see follow-up-tracks: objection track]
```

---

## Principles

- **Send fewer, better emails.** 50 personalized emails outperform 500 generic ones.
- **Don't feature-dump.** One pain point, one outcome, one ask.
- **Respect their time.** Short, clear, easy to say yes or no to.
- **Test everything.** Subject lines, opening hooks, CTAs. Run for 20 sends before judging.
- **Track replies, not opens.** Open rates are vanity. Reply rate is the signal.
- **Human tone beats polished.** Sound like a person, not a company.

## Related Skills

- `gtm-strategy` — Define the ICP before writing outreach
- `mom-test` — Use the discovery call once you get a reply
- `follow-up-tracks` — Handle all follow-up after first contact
- `first-users` — Manual outreach tactics for very early stage
