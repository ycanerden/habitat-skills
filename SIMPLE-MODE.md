# Simple Mode - For Non-Technical Founders

**Purpose:** Make Habitat Skills accessible to non-technical founders by removing jargon, providing copy-paste templates, and guiding them step-by-step.

---

## How Simple Mode Works

### For Users

**Activation:**
Users can activate simple mode by saying:
- "Use simple mode"
- "I'm not technical, can you simplify?"
- "Give me copy-paste templates"

**What changes:**
1. **No jargon** - Technical terms explained in plain English
2. **Guided questions** - One question at a time, not overwhelming
3. **Copy-paste outputs** - Ready-to-use templates, not frameworks
4. **Visual progress** - Checklist showing what's done and what's next
5. **Next steps** - Always end with "Here's exactly what to do next"

---

## Implementation Guide for Skills

### Pattern 1: Detect Simple Mode

At the start of each skill, check if the user wants simple mode:

```markdown
## Detect Mode

If the user mentions:
- "simple"
- "not technical"
- "step by step"
- "templates"
- "I don't understand"

→ Switch to Simple Mode

In Simple Mode:
- Ask one question at a time
- Use analogies and plain English
- Provide copy-paste templates
- Show progress checklist
```

### Pattern 2: Simplify Language

**Complex (default mode):**
"I'll analyze your positioning strategy using the Jobs-to-be-Done framework to identify differentiation opportunities."

**Simple mode:**
"I'll help you figure out what makes your product different from competitors. Think of it like explaining why someone should choose you over them."

### Pattern 3: Guided Questions (One at a Time)

**Default mode:**
Asks 5 questions upfront

**Simple mode:**
Asks 1 question → User answers → Next question

**Example:**
```
Agent: What's your product in one sentence?
User: A project management tool for designers
Agent: Great! Who are your main competitors?
User: Notion, Asana
Agent: Perfect. What do they struggle with that you solve?
...
```

### Pattern 4: Copy-Paste Templates

**Default mode:**
"Create an email sequence with 5 touchpoints: welcome, value demonstration, case study, urgency, final offer."

**Simple mode:**
"Here are 5 emails you can copy and customize:

**Email 1 - Welcome (Send immediately)**
```
Subject: Welcome to [Your Product]! Here's what to do first.

Hi [Name],

Thanks for signing up! Here's how to get started in 60 seconds:

1. [Action 1]
2. [Action 2]
3. [Action 3]

Need help? Just reply to this email.

[Your Name]
```

**Copy this email, replace the brackets, and send it.**"

### Pattern 5: Visual Progress

Show a checklist after each step:

```
✅ Strategy created
✅ Social posts written
⏳ Email sequence (in progress)
⏳ Landing page copy
⏳ Launch checklist
```

### Pattern 6: Always Include Next Steps

End every output with:

```
## What to Do Next

1. [Specific action with copy-paste example]
2. [Specific action with copy-paste example]
3. [Specific action with copy-paste example]

Need help with step 1? Say "help me with [X]" and I'll guide you.
```

---

## Example: Launch Strategy in Simple Mode

### Default Mode Output

```
# Launch Strategy Framework

## Pre-Launch Phase (2 weeks before)
1. Build anticipation through teaser campaign
2. Recruit early advocates
3. Prepare launch assets

## Launch Day Tactics
- Product Hunt launch optimization
- Coordinated social amplification
- Outreach to relevant communities

## Metrics & Optimization
...
```

### Simple Mode Output

```
# Your Launch Plan (Step-by-Step)

I'm going to help you launch DevMetrics in 2 weeks. Here's what we'll do:

## Week 1: Get Ready

**Step 1: Tell people it's coming**
- Post on Twitter: "Launching something new in 2 weeks for engineering managers 👀"
- Send email to your beta users: "You're getting early access next week"
- **Why:** Builds excitement and gets people waiting

**Copy-paste this tweet:**
"🚀 Launching DevMetrics in 2 weeks

Real-time GitHub analytics for engineering managers.
See PR velocity, code review time, and team productivity.

Set up in 30 seconds.

Want early access? Drop your email 👇"

**Step 2: Get 10 people to share your launch**
- Ask your beta users: "Will you share this on launch day?"
- Offer early access or a free month
- **Why:** More people sharing = more visibility

**Copy-paste this message to beta users:**
"Hey [Name],

DevMetrics is launching on Product Hunt in 2 weeks! Would you be willing to share it with your network when it goes live?

If you do, I'll extend your free access for another month as a thank you.

Let me know!
[Your Name]"

---

## Week 2: Launch Day

**Step 3: Launch on Product Hunt**
- Post at 12:01 AM PST (when Product Hunt resets)
- **Why:** More time to collect upvotes

**Copy-paste this Product Hunt description:**
"DevMetrics - Real-time analytics for GitHub repos

😤 The problem: Engineering managers waste hours creating status reports
✨ The solution: DevMetrics auto-tracks PR velocity, code review time, and team productivity
⚡ The magic: Connect GitHub in 30 seconds, see data immediately

Perfect for startups with 10-50 person dev teams.

Try it free: [your link]"

**Step 4: Share everywhere (within 2 hours of launch)**
Post on:
- Twitter (use the tweet template above)
- LinkedIn (share with your network)
- Dev communities (Dev.to, Hashnode, Hacker News)

**Why:** Product Hunt ranks by upvotes in first 24 hours. More shares = more upvotes.

---

## After Launch

**Step 5: Follow up with everyone who signed up**
Send this email within 24 hours:

**Copy-paste this email:**
"Subject: You're in! Here's how to get started with DevMetrics

Hi [Name],

Thanks for checking out DevMetrics on Product Hunt!

Here's how to get started:
1. Connect your GitHub repo (takes 30 seconds): [link]
2. See your team's metrics in real-time
3. Share insights with your team

Questions? Just reply to this email.

[Your Name]"

---

## Your Launch Checklist

Use this to track your progress:

**Week 1:**
- [ ] Post teaser on Twitter
- [ ] Email beta users for support
- [ ] Get 10 people to commit to sharing

**Week 2:**
- [ ] Prepare Product Hunt post
- [ ] Launch at 12:01 AM PST
- [ ] Share on Twitter, LinkedIn, Dev.to within 2 hours
- [ ] Respond to all comments on Product Hunt

**After launch:**
- [ ] Send welcome email to all signups
- [ ] Track conversion rate (signups → paid)
- [ ] Ask for feedback

---

## What to Do Next

1. **Copy the tweet template above** and schedule it for 2 weeks from today
2. **Copy the beta user message** and send it to your 50 beta users
3. Say **"help me write the Product Hunt post"** and I'll create it for you

Which do you want to do first?
```

---

## Simple Mode Templates Library

Create reusable templates for common tasks:

### Email Templates
- Welcome email
- Product launch email
- Re-engagement email
- Feedback request email

### Social Templates
- Twitter launch thread
- LinkedIn announcement
- Product Hunt description

### Copy Templates
- Landing page hero section
- Pricing page value props
- Feature descriptions

**Location:** `/templates/` directory with markdown files

---

## Skills That Should Support Simple Mode

**Priority 1 (MVP):**
- `launch-strategy` - Most requested, high impact
- `social-content` - Templates are easy to provide
- `email-sequence` - Copy-paste emails
- `copywriting` - Landing page templates

**Priority 2 (Post-launch):**
- `pricing-strategy` - Simplify pricing research
- `seo-audit` - Plain English SEO fixes
- `competitor-alternatives` - Comparison page templates

**Priority 3 (Future):**
- All other skills

---

## How to Test Simple Mode

### Test Case 1: Complete Beginner
**Persona:** Non-technical founder, first time launching a product

**Test flow:**
1. User: "I'm launching my product next week but I'm not technical. Can you help?"
2. Agent: *[Activates simple mode]*
3. Agent: "What's your product in one sentence?"
4. User: "A CRM for real estate agents"
5. Agent: *[Delivers step-by-step launch plan with copy-paste templates]*

**Success criteria:**
- No jargon used
- User can follow without asking for clarification
- Templates are immediately usable

### Test Case 2: Overwhelmed by Framework
**Persona:** Technical founder but overwhelmed by marketing jargon

**Test flow:**
1. User: "Help me with SEO"
2. Agent: *[Delivers technical SEO audit]*
3. User: "This is too complex, can you simplify?"
4. Agent: *[Switches to simple mode]*
5. Agent: "Here are 3 things to fix on your website, in plain English..."

**Success criteria:**
- Agent detects user confusion
- Switches modes smoothly
- Provides actionable, jargon-free fixes

---

## Simple Mode Activation Rules

**Auto-activate simple mode if user says:**
- "I'm not technical"
- "Can you simplify?"
- "I don't understand"
- "Step by step"
- "Give me templates"
- "What does [jargon word] mean?"

**Stay in simple mode unless:**
- User says "I want more detail"
- User asks technical questions
- User says "switch to advanced mode"

---

## Conversion Path

**Goal:** Start in simple mode, gradually introduce complexity as user gets comfortable.

**Stage 1: First interaction**
→ Simple mode by default for new users

**Stage 2: User completes first task**
→ Offer: "Want to learn the advanced version of this skill?"

**Stage 3: User ready for frameworks**
→ Switch to default mode with full frameworks

**Stage 4: Power user**
→ User can chain skills, use advanced features

---

## FAQ for Simple Mode

**Q: Will this make the output worse?**
A: No. Simple mode still delivers the same value, just packaged differently. Templates are based on proven frameworks.

**Q: How do we maintain both modes?**
A: Each skill has two output formats: (1) Framework-based (default), (2) Template-based (simple). Same underlying logic.

**Q: What if a user starts in simple mode but wants more depth?**
A: Always offer: "Want more detail? Say 'explain the framework' and I'll show you the strategy behind this."

---

## Implementation Checklist

- [ ] Add simple mode detection to CLAUDE.md
- [ ] Create templates library in `/templates/`
- [ ] Update priority skills with simple mode support:
  - [ ] launch-strategy
  - [ ] social-content
  - [ ] email-sequence
  - [ ] copywriting
- [ ] Test with non-technical users (3 people minimum)
- [ ] Document common questions and add to FAQ
- [ ] Add "Simple Mode" toggle to README

---

**Next step:** Start with `launch-strategy` skill—it's the most requested and highest impact.
