# What's New in Habitat Skills

**Last updated:** February 10, 2026

---

## 🎉 Major Updates

All three proposed improvements have been implemented and are ready for Friday's demo!

---

## 1. Autonomous Research with Firecrawl 🔍

**What it does:**
Agent autonomously scrapes competitor websites to extract positioning, pricing, features, and target audience—no manual research required.

**New skill:**
- `portfolio-research` - Scrape and analyze competitors using Firecrawl

**Example:**
```
User: "Research Notion, Coda, and Airtable"
Agent: [Scrapes all three sites]
Agent: [Delivers competitive analysis with pricing, features, differentiation angles]
```

**How to enable:**
1. Get a free API key from [firecrawl.dev](https://firecrawl.dev)
2. Add it to `~/.claude/mcp-config.json` (file already created)
3. Restart Claude Code

See: [FIRECRAWL-SETUP.md](FIRECRAWL-SETUP.md) for step-by-step instructions.

---

## 2. Simple Mode for Non-Technical Founders 👥

**What it does:**
Non-technical founders get copy-paste templates, guided questions, and jargon-free outputs.

**How to activate:**
Say "use simple mode", "I'm not technical", or "give me templates"

**What changes:**
- ✅ No jargon (technical terms explained with analogies)
- ✅ One question at a time (not overwhelming)
- ✅ Copy-paste templates (ready to use)
- ✅ Visual progress (checklists)
- ✅ Clear next steps ("Here's exactly what to do next")

**New templates library:**
- Email templates: 5 launch emails (`templates/email/launch-sequence.md`)
- Social templates: Twitter, LinkedIn, Reddit, HN (`templates/social/product-hunt-launch.md`)
- Copy templates: 7 landing page hero formats (`templates/copy/landing-page-hero.md`)

**Example difference:**

**Default mode:**
"Create an email sequence with 5 touchpoints: welcome, value demonstration, case study, urgency, final offer."

**Simple mode:**
"Here are 5 emails you can copy and customize:

**Email 1 - Welcome**
```
Subject: Welcome to [Your Product]!
[Copy-paste template with brackets to fill in]
```

Copy this, replace the brackets, and send it."

See: [SIMPLE-MODE.md](SIMPLE-MODE.md) for implementation guide.

---

## 3. Demo-Ready Materials 🎯

**What's included:**
Complete materials for Friday's accelerator presentation—demo script, sample project, video outline, and backup plan.

**Files created:**
- `DEMO-SCRIPT.md` - Word-for-word presentation script (8-10 minutes)
- `demo-project/` - Sample project (DevMetrics) with pre-filled context
- `demo-project/VIDEO-OUTLINE.md` - 15-20 second backup video plan
- `demo-project/README.md` - Setup instructions and troubleshooting

**Demo flow:**
1. **The Hook (30s):** Founder pain point ("You're launching but don't know how to get users")
2. **Instant Value (2min):** Show `launch-strategy` skill in action
3. **The Power (3min):** Chain skills together (`launch-strategy` → `social-content` → `email-sequence`)
4. **The Vision (2min):** Live Firecrawl demo (scrape competitors, analyze positioning)
5. **Q&A:** Backup examples ready

**Sample product (DevMetrics):**
- Real-time analytics for GitHub repositories
- Target: Engineering managers at startups
- Competitors: LinearB, Haystack, Swarmia
- Differentiator: 30-second setup vs enterprise complexity

See: [DEMO-SCRIPT.md](DEMO-SCRIPT.md) for full presentation guide.

---

## Files Overview

### New Files
| File | Purpose |
|------|---------|
| `skills/portfolio-research/SKILL.md` | Autonomous competitor research skill |
| `~/.claude/mcp-config.json` | Firecrawl MCP configuration |
| `SIMPLE-MODE.md` | Implementation guide for simple mode |
| `templates/email/launch-sequence.md` | 5 launch email templates |
| `templates/social/product-hunt-launch.md` | Social media templates (Twitter, LinkedIn, etc.) |
| `templates/copy/landing-page-hero.md` | 7 landing page hero section formats |
| `DEMO-SCRIPT.md` | Word-for-word presentation script |
| `demo-project/*` | Sample project for demo |
| `FIRECRAWL-SETUP.md` | Firecrawl setup instructions |
| `IMPROVEMENT-ROADMAP.md` | Complete roadmap with implementation status |
| `WHATS-NEW.md` | This file |

### Updated Files
| File | What Changed |
|------|--------------|
| `README.md` | Added "What's New" section, `portfolio-research` skill |
| `CLAUDE.md` | No changes needed (conventions still apply) |

---

## Quick Start Guide

### For Technical Founders

**1. Enable Firecrawl (optional but recommended):**
```bash
# Get API key from firecrawl.dev
# Add to ~/.claude/mcp-config.json
# Restart Claude Code
```

**2. Try the new skill:**
```
Research my top 3 competitors and show me how to differentiate
```

**3. Use templates:**
```
Use simple mode to create launch emails
```

---

### For Non-Technical Founders

**1. Activate simple mode:**
```
I'm not technical, can you help me launch my product?
```

**2. Follow the guided questions:**
Agent will ask one question at a time, then deliver copy-paste templates.

**3. Use the templates:**
Copy the templates, replace the `[brackets]`, and use them immediately.

---

### For the Demo (Friday)

**1. Setup:**
```bash
cd demo-project
# Open in Claude Code
```

**2. Test the demo flow:**
```
Help me plan a launch strategy for DevMetrics
```

**3. Practice the Firecrawl demo:**
```
Research LinearB, Haystack, and Swarmia
```

See: [DEMO-SCRIPT.md](DEMO-SCRIPT.md) for full instructions.

---

## What's Next

**Before Friday:**
- [ ] Get Firecrawl API key and test live scraping
- [ ] Record 15-20 second backup video (optional)
- [ ] Practice presentation 2-3 times

**After Friday:**
- [ ] Collect feedback from Yannick and jury
- [ ] Integrate simple mode into priority skills
- [ ] Test with non-technical users
- [ ] Update existing skills to leverage `portfolio-research` data

---

## Breaking Changes

**None.** All changes are additive and backward-compatible.

Existing skills work exactly as before. New features are opt-in:
- Firecrawl requires manual setup
- Simple mode activates on user request
- Templates are optional

---

## FAQ

**Q: Do I need Firecrawl to use Habitat Skills?**
A: No. Most skills work without it. Only `portfolio-research` requires it for autonomous scraping. Without Firecrawl, the skill falls back to web search or manual research.

**Q: How do I activate simple mode?**
A: Just say "use simple mode", "I'm not technical", or "give me templates". The agent will switch automatically.

**Q: Are the templates customizable?**
A: Yes. All templates have `[brackets]` where you fill in your product details. You can also edit the templates in `templates/` to create your own.

**Q: What if I'm demoing on Friday and internet fails?**
A: Use the backup materials in `demo-project/demo-assets/` or show the pre-recorded video from `VIDEO-OUTLINE.md`.

**Q: Can I contribute new templates?**
A: Yes! Add them to `templates/` and submit a PR. We welcome contributions.

---

## Feedback

Found a bug? Have a suggestion? Want to contribute?

- **GitHub Issues:** [github.com/ycanerden/habitat-skills/issues](https://github.com/ycanerden/habitat-skills/issues)
- **Habitat Community:** [joinhabitat.eu](https://joinhabitat.eu)

---

**Happy launching! 🚀**
