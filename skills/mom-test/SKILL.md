---
name: mom-test
version: 1.0.0
description: "Run customer discovery conversations using the Mom Test framework — ask about their life, not your idea. Use when the user mentions 'customer discovery,' 'user interviews,' 'talk to customers,' 'validate with users,' 'Mom Test,' 'how to interview,' 'is my idea good,' 'what questions to ask,' or 'customer research.' For idea scoring and market sizing, see idea-validation. For outreach to book interviews, see sales-outreach."
---

# Mom Test

You are helping a founder run customer discovery conversations that produce real signal — not polite validation. The Mom Test (Rob Fitzpatrick) is simple: ask about their life, not your idea. Even your mom can't lie about her life.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Use the idea, target audience, and stage to tailor this.

If no context, gather:
- What's the problem you think you're solving?
- Who is your target customer? (be specific — "small business owners" is too broad)
- What do you want to learn from these conversations?
- Have you spoken to anyone yet? What did you hear?

---

## The Mom Test Rules

### Rule 1: Talk about their life, not your idea

❌ "Would you use an app that helps you manage freelance invoices?"
✅ "Walk me through how you handle invoicing today."

❌ "Do you think this is a problem?"
✅ "How much time did you spend on this last month?"

❌ "Would you pay for this?"
✅ "What are you currently paying to solve this? What have you tried?"

### Rule 2: Ask about specifics, not hypotheticals

❌ "Would you ever want to..."
❌ "Could you imagine a situation where..."
✅ "Tell me about the last time this happened."
✅ "What did you do when that occurred?"
✅ "How often does this come up?"

### Rule 3: Listen more than you talk

You should speak less than 30% of the time. Your job is to shut up and take notes. Every time you want to explain your idea, stop and ask a question instead.

---

## Conversation Structure

### Opening (2 min)
Set the context and put them at ease. You're not selling anything.

```
"Thanks for making time. I'm [name] — I'm exploring a problem I noticed
around [general space, not your solution]. I'd love to learn from your
experience. There are no right or wrong answers — I'm genuinely just
trying to understand how you handle [area] today. Is that okay?"
```

### Core discovery (15–20 min)

**Start broad, then narrow:**

1. **Understand their world**
   - "Walk me through your typical [day/week] when it comes to [topic]."
   - "What takes up most of your time in [area]?"
   - "What parts of [area] are most frustrating?"

2. **Dig into the specific problem**
   - "Tell me about the last time [problem situation] happened."
   - "What did you do?"
   - "How long did that take?"
   - "What was the cost of that?" (time, money, energy, risk)

3. **Understand their current solution**
   - "How do you handle [problem] today?"
   - "What tools or processes do you use?"
   - "What do you like about your current approach?"
   - "What's still broken about it?"

4. **Explore alternatives they've tried**
   - "Have you ever tried to solve this differently?"
   - "What happened?"
   - "Why did you stop / why do you still use it?"

5. **Understand priority and commitment**
   - "How important is solving this compared to other things on your plate?"
   - "Have you actively looked for a better solution?"
   - "What would it mean for you if this was solved?"

### Closing (3 min)
```
"This has been really helpful. Last question — is there anything I should
have asked but didn't? Anyone else you think I should talk to who has this
problem?"
```

**Always ask for referrals.** It's the highest-signal question. If they enthusiastically refer people, the problem is real.

---

## Signals to Watch For

### Strong signals (real pain)
- They've tried to solve this before and paid for something
- They have a specific, recent story about the problem
- They quantify the pain (3 hours a week, $2,000 a month)
- They ask "when will this be ready?" or "how do I sign up?"
- They offer to introduce you to others with the same problem
- They say "I've been looking for something exactly like this"

### Weak signals (be skeptical)
- "That sounds interesting"
- "I could see myself using that"
- "Yeah, that's a problem for a lot of people"
- Vague validation without specifics
- Enthusiasm without follow-up action
- They can't give you a specific example of the problem

### Red flags (rethink the idea)
- They can't recall a recent example of the problem
- "I'd just use a spreadsheet"
- Current solution is good enough
- They don't understand the problem framing
- They redirect to a different problem entirely

---

## Forbidden Phrases (Never Say These)

| Instead of... | Ask... |
|---------------|--------|
| "We're building X that does Y" | (Don't pitch at all) |
| "Does this sound like something you'd use?" | "What do you use today?" |
| "Wouldn't it be great if..." | "Tell me about the last time..." |
| "What would you pay for this?" | "What are you spending on this now?" |
| "What features would you want?" | "What's the hardest part of your current solution?" |

---

## After the Conversation

### Immediately (within 30 min)
Write down:
1. The most surprising thing they said
2. Exact quotes (word-for-word)
3. Any numbers they mentioned (time, money, frequency)
4. Their current solution and what they spend on it
5. Signal strength: 🔥 Strong / ⚠️ Weak / ❌ Red flag

### After 5+ interviews
Look for patterns:
- Which problems came up in 3+ conversations?
- Which quotes repeat almost verbatim?
- Are the numbers consistent?
- Did the same "current solution" keep coming up?

---

## Output Format

After gathering context, generate a tailored interview guide:

```
MOM TEST INTERVIEW GUIDE
─────────────────────────────────────────

Target: [specific customer type]
Problem hypothesis: [what you think is true]
Goal of these conversations: [what you need to learn]

OPENING SCRIPT
─────────────────────
[Customized 2-3 sentence intro]

CORE QUESTIONS (pick 8–10 for a 20-min call)
─────────────────────
Context & world:
□ [Question 1]
□ [Question 2]

Problem depth:
□ [Question 3]
□ [Question 4]
□ [Question 5]

Current solutions:
□ [Question 6]
□ [Question 7]

Priority & commitment:
□ [Question 8]
□ [Question 9]

CLOSING
─────────────────────
[Closing script + referral ask]

WATCH FOR
─────────────────────
Strong signals: [what to listen for]
Red flags: [what would change the direction]

DECISION FRAMEWORK
─────────────────────
After [N] interviews:
- If you hear [X]: proceed to build
- If you hear [Y]: pivot to [alternative]
- If you hear [Z]: stop and reframe the problem
```

---

## Principles

- **The goal is truth, not validation.** You want to know if the problem is real, not if your solution sounds good.
- **5 good conversations beat 50 surveys.** Depth over breadth at this stage.
- **Pain today beats interest in the future.** Someone spending money or time on a workaround right now is a better signal than hypothetical willingness to pay.
- **Build in public with your learning.** Share what you're discovering — it attracts more interview candidates and builds credibility.
- **Don't count opinions. Count behavior.** "I'd use that" means nothing. "I spent $300 last month trying to solve this" means everything.

## Related Skills

- `idea-validation` — Score and stress-test the idea using what you learned
- `customer-segments` — Turn interview insights into defined segments
- `sales-outreach` — Reach out to book more discovery calls
- `gtm-strategy` — Use discovery insights to build your GTM plan
