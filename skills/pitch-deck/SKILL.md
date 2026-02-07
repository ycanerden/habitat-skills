---
name: pitch-deck
version: 1.0.0
description: "Create a compelling pitch — from 30-second elevator pitch to full demo script. Use when the user mentions 'pitch,' 'pitch deck,' 'elevator pitch,' 'demo script,' 'how to present my idea,' 'investor pitch,' 'demo day,' '30-second pitch,' or 'pitch practice.' For idea-level validation, see idea-validation. For landing page copy, see landing-page."
---

# Pitch Deck

You are helping a founder create a clear, compelling pitch for their startup. This covers everything from a 30-second elevator pitch to a full demo presentation. The goal is clarity and confidence — not polish.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Use the idea, audience, problem, solution, and competitive info to auto-fill as much of the pitch as possible.

If no context exists, gather:
- What are you building? (one sentence)
- What problem does it solve?
- Who is it for?
- Do you have a working prototype or MVP?
- What's the pitch for? (Habitat demo, investor meeting, casual conversation, pitch competition)

## Pitch Formats

### 1. The 30-Second Pitch

For: Habitat evening demos, casual conversations, networking events.

**Structure (4 sentences):**

```
[PROBLEM]: [Specific audience] struggles with [specific problem].
[SOLUTION]: [Product name] [what it does in one sentence].
[PROOF]: [One concrete result, metric, or demonstration].
[ASK]: [What you want from the listener].
```

**Example:**
> Freelance designers spend 5+ hours a week chasing late payments.
> InvoiceBot sends automatic payment reminders and follows up until clients pay.
> In our first week, 3 designers recovered over €2,000 in overdue invoices.
> I'm looking for 10 more designers to test it — know anyone?

**Rules:**
- No jargon. If your mom can't understand it, simplify.
- One specific number or result. "3 designers recovered €2,000" beats "we help freelancers."
- The ask should match the context. At Habitat: "Try it tonight." With investors: "We're raising €500K."
- Practice saying it out loud. If it takes more than 30 seconds, cut words.

### 2. The 2-Minute Pitch

For: Demo day, pitch competitions, investor intros.

**Structure (6 parts, ~20 seconds each):**

```
1. HOOK — Start with a surprising fact, question, or story
2. PROBLEM — The pain point (make them feel it)
3. SOLUTION — What you built (show, don't tell)
4. TRACTION — What's happened so far (users, revenue, feedback)
5. WHY NOW — Why this moment matters (market shift, new technology, regulation)
6. ASK — What you need (funding, users, advice, introductions)
```

**Rules:**
- Open with the hook, not "Hi, I'm [name] and we're building..."
- Show the product if possible (live demo or screenshot)
- One slide per section maximum (if using slides)
- End on the ask — don't trail off

### 3. The Demo Script

For: Live product demonstrations at Habitat evenings or demo days.

**Structure:**

```
1. SETUP (15 sec) — "Imagine you're a [target user] and you need to [task]..."
2. CURRENT WAY (15 sec) — "Today, you'd have to [painful current process]..."
3. OUR WAY (60 sec) — Live walkthrough of the core user flow
4. RESULT (15 sec) — "And now [the outcome]. That took [time] instead of [old time]."
5. CLOSE (15 sec) — "We launched tonight. [X] people have signed up. Try it at [URL]."
```

**Demo rules:**
- Practice the exact clicks beforehand. No fumbling.
- Have a backup plan (screenshots) if wifi dies or the app crashes.
- Show the ONE core flow. Don't show settings, admin panels, or edge cases.
- Narrate what you're doing: "Now I'm clicking [X] and you'll see [Y]."
- End with the live URL on screen.

### 4. The Full Pitch Deck (10-12 slides)

For: Investor meetings, accelerator applications.

**Slide structure:**

| Slide | Content | Time |
|-------|---------|------|
| 1. **Title** | Product name, one-line description, your name | 5 sec |
| 2. **Problem** | The pain point with a specific story or data | 30 sec |
| 3. **Solution** | What you built, screenshot or demo | 30 sec |
| 4. **Demo** | Live walkthrough or key screenshots | 60 sec |
| 5. **How it works** | 3-step process or architecture | 20 sec |
| 6. **Traction** | Users, revenue, growth, testimonials | 30 sec |
| 7. **Market** | TAM/SAM/SOM with sources | 20 sec |
| 8. **Business model** | How you make money, pricing | 20 sec |
| 9. **Competition** | 2x2 positioning map | 20 sec |
| 10. **Team** | Why you're the right team | 15 sec |
| 11. **Ask** | How much, what for, timeline | 15 sec |
| 12. **Contact** | URL, email, QR code | 5 sec |

**Rules:**
- Max 10 words per slide. The slides support your talk — they're not the talk.
- One idea per slide.
- Use screenshots, not mockups (if you have a product).
- No bullet points on slides. Tell a story.

## Objection Handling

Prepare for the top 3 questions you'll get:

**Common objections and how to handle them:**

| Objection | Bad Response | Good Response |
|-----------|-------------|---------------|
| "How is this different from [competitor]?" | "We have more features" | "[Competitor] focuses on [X]. We solve [Y] for [specific audience] because [specific reason]." |
| "How do you make money?" | "We'll figure that out later" | "We charge [amount] per [unit]. Our first [N] users pay [amount]." |
| "What if [big company] builds this?" | "They won't" | "They could, but [specific reason they won't focus on this niche]. By then we'll have [moat]." |
| "How big is the market?" | "It's huge" | "[Specific number] of [specific people] spend [specific amount] on [category] today." |
| "Why now?" | "It's a good idea" | "[Specific market shift] — [new technology / regulation / behavior change] makes this possible now." |

**Prep method:**
1. Write down the 3 hardest questions someone could ask
2. Write a 2-sentence answer for each
3. Practice saying them out loud
4. If you can't answer one — that's your riskiest assumption. Address it before the pitch.

## Habitat Evening Demo Guide

If you're pitching at a Habitat evening, here's the specific format:

**You have 2-3 minutes. Use this structure:**

```
[15 sec] "We built [product name]. It helps [audience] do [outcome]."
[15 sec] "The problem: [one sentence about the pain]."
[60 sec] [LIVE DEMO — show the core flow on your screen]
[15 sec] "Tonight we [what you accomplished — launched, got signups, etc.]."
[15 sec] "Try it at [URL]. We're looking for [specific ask]."
```

**Before your demo:**
- [ ] Core flow works end-to-end (test it twice)
- [ ] URL is live and accessible
- [ ] You can explain it in one sentence without jargon
- [ ] You know your first line (don't wing the opening)
- [ ] Backup screenshots ready in case the app crashes

## Output Format

### Pitch Package

```
PITCH PACKAGE
─────────────────────────────────────────

Product: [name]
Audience: [who]
Pitch context: [where you're presenting]

30-SECOND PITCH
─────────────────────
[Full 30-second pitch script]

DEMO SCRIPT
─────────────────────
Setup: [what to say]
Current way: [the pain]
Our way: [narrate the demo steps]
Result: [the payoff]
Close: [the ask]

OBJECTION PREP
─────────────────────
Q: [Likely question 1]
A: [Prepared answer]

Q: [Likely question 2]
A: [Prepared answer]

Q: [Likely question 3]
A: [Prepared answer]

PRE-DEMO CHECKLIST
─────────────────────
□ Core flow tested
□ URL is live
□ One-sentence description memorized
□ Opening line practiced
□ Backup screenshots ready
```

## Principles

- **Clarity over completeness.** A pitch that explains one thing well beats a pitch that mentions everything.
- **Show, don't tell.** "Here, let me show you" is the most powerful sentence in a demo.
- **Specific over impressive.** "3 users in 2 hours" is more credible than "massive market opportunity."
- **Practice the opening.** The first 10 seconds determine if people pay attention. Know your first line cold.
- **Match the ask to the audience.** At Habitat: "Try it." With investors: "We're raising." With peers: "What do you think?"
- **Silence is okay.** During a live demo, let the product speak. Don't fill every second with words.

## Related Skills

- `founder-context` — Set up context that auto-fills the pitch
- `idea-validation` — Validate before pitching (know your weak spots)
- `competitor-research` — Prep for "how are you different?" questions
- `landing-page` — Build the page your pitch URL points to
- `first-users` — What to do after the pitch lands
