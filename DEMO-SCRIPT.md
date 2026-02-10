# Habitat Skills - Demo Script (Friday Presentation)

**Total time:** 8-10 minutes
**Format:** Live demo + backup video (15-20 seconds)
**Audience:** Startup accelerator class + jury

---

## Pre-Demo Setup (Do Before Presentation)

**Tech setup:**
- [ ] Open Claude Code in `demo-project/` directory
- [ ] Ensure `.claude/founder-context.md` is pre-filled (see sample below)
- [ ] Test Firecrawl MCP is working (if using)
- [ ] Have backup screenshots ready in `demo-assets/`
- [ ] Record 15-20 second video showing the skill in action (backup if internet fails)

**Presentation setup:**
- [ ] Slides: Problem → Solution → Demo → Vision
- [ ] Printed one-pager with QR code to GitHub repo
- [ ] Backup examples ready (3 different skills)

---

## Opening (30 seconds)

### Slide 1: The Problem

**Say:**
"You're a founder. You just built your MVP. Now you need to launch it.

You Google 'how to launch a product' and get 47 blog posts with generic advice. You ask ChatGPT and it gives you a wall of text. You hire a marketing consultant for $5,000.

**Or... you use Habitat Skills.**"

---

## Stage 1: The Hook (2 minutes)

### Slide 2: What is Habitat Skills?

**Say:**
"Habitat Skills is an AI agent framework for founders. Instead of generic AI, you get structured playbooks for every marketing and growth challenge.

Think of it like this: ChatGPT is a smart intern. Habitat Skills is a marketing team."

**On screen:**
- Show the skills directory (25+ skills)
- Highlight categories: Marketing, SEO, CRO, Growth

**Say:**
"Each skill is a framework. Launch strategy. Pricing. SEO. Competitor research. Copywriting. All optimized for founders."

---

## Stage 2: Instant Value Demo (3 minutes)

### Live Demo: Launch Strategy Skill

**Setup:**
- Switch to Claude Code terminal
- Show empty terminal (fresh session)

**Say:**
"Let me show you. I'm launching a new SaaS tool for developers. I need a launch strategy."

**Type in Claude:**
```
Help me plan a launch strategy for my developer tool
```

**Agent responds:**
*[Reads founder-context.md, then delivers launch strategy framework]*

**Point out:**
1. "Notice: No 20 questions. It just works."
2. "It read my product context automatically."
3. "This is a structured framework, not generic advice."

**Say:**
"Here's my launch strategy: Product Hunt, dev communities, Twitter launch, email sequence. Each with specific tactics."

**Scroll through output, highlight:**
- Pre-launch checklist
- Launch day playbook
- Post-launch momentum tactics

**Say:**
"This would take a consultant days to create. It took 10 seconds."

---

## Stage 3: The Power - Chaining Skills (3 minutes)

### Demo: Show How Skills Work Together

**Say:**
"But here's where it gets powerful. Skills chain together."

**Type in Claude:**
```
Now create social posts for my Product Hunt launch
```

**Agent responds:**
*[social-content skill creates Twitter thread, LinkedIn post, launch announcement]*

**Say:**
"Now I have social posts. Let me get email copy too."

**Type in Claude:**
```
Draft a launch email sequence for my waitlist
```

**Agent responds:**
*[email-sequence skill creates 3-email launch series]*

**Say:**
"In 60 seconds, I went from zero to a complete launch campaign:
✅ Strategy
✅ Social posts
✅ Email sequence

This is what I mean by 'like having a marketing team in Claude.'"

---

## Stage 4: The Vision - Agentic Research (2 minutes)

### Slide 3: What's Next

**Say:**
"Right now, you have to provide context manually. But we're adding autonomous research with Firecrawl."

### Live Demo (or Video): Portfolio Research

**Say:**
"Watch this."

**Type in Claude:**
```
Research Notion, Coda, and Airtable. Show me how to differentiate.
```

**Agent:**
*[Uses Firecrawl to scrape all three websites]*
*[Extracts positioning, pricing, features]*
*[Delivers competitive analysis report in 30 seconds]*

**Say:**
"It just scraped three competitor websites, analyzed their positioning, pricing, and features, and told me exactly how to differentiate.

This is what founders need: not generic AI, but AI that does the work."

### Backup Option (If Firecrawl Demo Fails)

**Say:**
"We're also adding autonomous research. Imagine typing 'analyze my top 5 competitors' and the agent scrapes their websites, extracts positioning and pricing, and delivers a competitive analysis—all in 30 seconds."

**Show:** 15-20 second pre-recorded video of Firecrawl in action

---

## Closing (1 minute)

### Slide 4: Traction & Next Steps

**Say:**
"Habitat Skills is open source. 25+ skills. Built for founders who need marketing frameworks, not generic AI.

We're adding:
- Autonomous research (like you just saw)
- Simple mode for non-technical founders
- More skills (100+ planned)

If you're building a startup and need help with marketing, this is for you."

**Show QR code:**
"GitHub repo: github.com/canerden/habitat-skills. Try it this weekend."

---

## Q&A Preparation

### Expected Questions & Answers

**Q: "How is this different from ChatGPT?"**
A: "ChatGPT is generic. Habitat Skills is structured frameworks. ChatGPT gives you advice. Habitat Skills gives you action plans. Plus, it chains skills together—like a marketing team, not an intern."

**Q: "What if I'm not technical? Can I use this?"**
A: "Great question. Right now it's built for technical founders. But we're adding a 'simple mode' that removes all jargon and provides copy-paste templates. You'll be able to use it like a conversation, no coding required."

**Q: "Can it write my entire marketing plan?"**
A: "Yes. You can chain skills: `launch-strategy` → `social-content` → `email-sequence` → `copywriting` → `seo-audit`. In 10 minutes, you have a complete plan."

**Q: "What's the business model?"**
A: "Right now it's open source. Long-term, we see three paths: (1) Freemium with premium skills, (2) SaaS version with templates, or (3) Marketplace for skill creators."

**Q: "How does the Firecrawl integration work?"**
A: "Firecrawl is a web scraping API. We use it via the Model Context Protocol (MCP). When you ask to research a competitor, the agent scrapes their site, extracts structured data, and feeds it into the analysis. All autonomous."

**Q: "Who is this for?"**
A: "Technical founders building SaaS products. Especially solo founders who can't afford a marketing team. Eventually, we'll expand to non-technical users too."

---

## Backup Examples (If Time Permits)

### Example 1: Pricing Strategy
**User:** "Help me price my developer tool"
**Agent:** *[pricing-strategy skill delivers Van Westendorp analysis, tier recommendations, packaging advice]*

### Example 2: SEO Audit
**User:** "Audit my landing page for SEO"
**Agent:** *[seo-audit skill checks meta tags, headings, schema, page speed, delivers fix list]*

### Example 3: Competitor Comparison Page
**User:** "Create a '[My Product] vs Notion' comparison page"
**Agent:** *[competitor-alternatives skill delivers modular comparison with features, pricing, use cases]*

---

## Video Outline (15-20 Seconds for Backup)

**Title:** "Habitat Skills: AI Marketing Team for Founders"

**Script:**
- 0-3s: Screen recording of typing "Help me plan a launch strategy"
- 4-8s: Show agent delivering structured framework
- 9-14s: Type "Research my competitors" → Firecrawl scrapes → analysis appears
- 15-18s: Text overlay: "25+ marketing skills. Built for founders. Open source."
- 19-20s: QR code + "Try it: github.com/canerden/habitat-skills"

**Editing notes:**
- Speed up screen recording (1.5x)
- Add subtitles (no voiceover needed)
- Upbeat background music
- Clean, minimal aesthetic

---

## Sample Founder Context (Pre-filled for Demo)

Create this file before the demo: `demo-project/.claude/founder-context.md`

```markdown
# Founder Context

## Product
**Name:** DevMetrics
**One-liner:** Real-time analytics for GitHub repositories
**What it does:** Tracks pull request velocity, code review time, and contributor activity. Helps engineering managers understand team productivity.

## Target Audience
- Engineering managers at startups (10-50 person teams)
- Technical founders
- DevOps teams

## Stage
- MVP built, 50 beta users
- Launching publicly in 2 weeks

## Competitors
- LinearB
- Haystack
- Swarmia

## Unique Value
- Fastest setup (connect GitHub in 30 seconds)
- Designed for small teams (not enterprise)
- Beautiful, simple dashboards

## Business Model
- Freemium: Free for 1 repo, $29/mo for 5 repos, $99/mo for unlimited
```

---

## Post-Demo Actions

**Immediately after:**
- [ ] Share GitHub link in chat
- [ ] Collect email addresses from interested people
- [ ] Note all questions and feedback

**Within 24 hours:**
- [ ] Send follow-up email with demo video
- [ ] Update roadmap based on feedback
- [ ] Post demo video on Twitter/LinkedIn

---

## Presenter Notes

**Energy:**
- Start strong with the problem (founders know this pain)
- Show, don't tell (live demo > slides)
- Keep it fast-paced (no pauses)

**Key message:**
"Habitat Skills is like having a marketing team in Claude. Structured frameworks, not generic advice."

**Tone:**
- Confident but not arrogant
- Founder-to-founder (you understand their pain)
- Show the vision (this is just the beginning)

**Timing:**
- If running long, skip Stage 3 (chaining demo)
- If running short, add a backup example

---

**Good luck! 🚀**
