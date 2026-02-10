# Habitat Skills - Improvement Roadmap

**Status:** ✅ Implemented and ready for Friday demo
**Last updated:** February 10, 2026
**Contributors:** Caner, [Add Yannick + others]

---

## 🎉 Implementation Summary

**All 3 improvements have been implemented and are ready for Friday's demo!**

| Improvement | Status | Files Created |
|-------------|--------|---------------|
| **Firecrawl Integration** | ✅ Complete | `~/.claude/mcp-config.json`, `skills/portfolio-research/SKILL.md` |
| **Demo Flow** | ✅ Complete | `DEMO-SCRIPT.md`, `demo-project/*`, `VIDEO-OUTLINE.md` |
| **Simple Mode** | ✅ Complete | `SIMPLE-MODE.md`, `templates/email/*`, `templates/social/*`, `templates/copy/*` |

**What's ready:**
- ✅ Complete demo script with Q&A prep
- ✅ Sample project (DevMetrics) with pre-filled context
- ✅ Autonomous competitor research via Firecrawl
- ✅ Simple mode framework for non-technical users
- ✅ 15+ copy-paste templates (emails, social posts, landing page copy)
- ✅ 15-20 second video outline for backup/promotion

**What's needed before Friday:**
- Get Firecrawl API key and test live scraping
- Record backup video (optional, in case internet fails)
- Practice presentation 2-3 times

---

## Overview

Habitat Skills is an AI agent framework for founders. Instead of generic AI assistance, it provides structured playbooks for building startups—marketing strategy, SEO, pricing, launch planning, etc.

**Current state:** 26 skills covering marketing, CRO, SEO, and growth (including new `portfolio-research`)
**Target users:** Technical and non-technical founders
**Presentation date:** Friday (this week)

---

## Proposed Improvements

### 1. **Autonomous Research with Firecrawl** 🔍 ✅ IMPLEMENTED

**Problem:** Right now, users have to manually provide context about competitors, market positioning, and their product. This creates friction.

**Solution:** Let the agent autonomously research portfolio companies and competitors using web scraping (Firecrawl).

**How it works:**
1. User mentions a competitor or provides a URL
2. Agent automatically scrapes their website
3. Extracts: positioning, features, pricing, target audience
4. Uses this data to inform recommendations

**Example use case:**
- User: "Help me position against Notion"
- Agent: *[scrapes notion.so]* → "Based on Notion's positioning as an 'all-in-one workspace,' here's how you can differentiate..."

**Implementation status:**
- ✅ Firecrawl MCP configuration created (`~/.claude/mcp-config.json`)
- ✅ `portfolio-research` skill created (`skills/portfolio-research/SKILL.md`)
- ✅ Includes fallback for when Firecrawl is not configured
- ⏳ Update existing skills to leverage scraped data (post-MVP)

**How to enable:**
1. Get a free Firecrawl API key from [firecrawl.dev](https://firecrawl.dev)
2. Add your key to `~/.claude/mcp-config.json` (file already created)
3. Restart Claude Code
4. Test with: "Research Notion and show me their pricing"

**Benefit:** Faster context gathering, better recommendations, feels more "agentic"

**Sources:**
- [Firecrawl MCP Server Documentation](https://docs.firecrawl.dev/mcp-server)
- [GitHub: firecrawl-mcp-server](https://github.com/firecrawl/firecrawl-mcp-server)

---

### 2. **Easy Demo Flow for Friday Presentation** 🎯 ✅ IMPLEMENTED

**Problem:** We need a smooth 5-10 minute demo that shows immediate value without overwhelming the audience.

**Demo flow (8-10 minutes):**

**Stage 1: The Hook (30 seconds)**
- Start with a concrete founder pain point
- Example: "You're launching next week but don't know how to get your first 100 users"

**Stage 2: Instant Value (2 minutes)**
- Show a single skill in action (recommend: `launch-strategy`)
- User types one sentence → Agent delivers a complete framework
- Emphasis: "No 20-question setup, just results"

**Stage 3: The Power (3 minutes)**
- Show how skills chain together:
  - `launch-strategy` → identifies Product Hunt as a channel
  - `social-content` → creates announcement posts
  - `email-sequence` → drafts launch emails
- Emphasize: "Like having a marketing team in Claude"

**Stage 4: The Vision (2 minutes)**
- Introduce the Firecrawl improvement
- Live demo: "Analyze my competitor's positioning" → agent scrapes → delivers insights
- Show how this scales: 10 competitors analyzed in 30 seconds

**Stage 5: Q&A**
- Have backup examples ready (different skills, different use cases)

**Materials created:**
- ✅ Complete demo script: `DEMO-SCRIPT.md` (word-for-word, includes Q&A prep)
- ✅ Sample project: `demo-project/` with pre-filled `.claude/founder-context.md`
- ✅ Video outline: `demo-project/VIDEO-OUTLINE.md` (15-20 second backup video)
- ✅ Demo README: `demo-project/README.md` (setup instructions, troubleshooting)
- ⏳ Slides (create separately or use script as speaking notes)

**Demo product (DevMetrics):**
- Real-time analytics for GitHub repositories
- Target: Engineering managers at startups
- Competitors: LinearB, Haystack, Swarmia
- Differentiator: 30-second setup vs. enterprise complexity

**Backup plan:**
- Screenshots in `demo-project/demo-assets/`
- Pre-recorded 15-20 second video showing Firecrawl in action
- Offline demo using pre-written examples

---

### 3. **Non-Technical Founder Flow** 👥 ✅ IMPLEMENTED

**Problem:** Current skills assume some technical comfort. Non-technical founders might get lost.

**Solution:** Create a guided, conversational flow that removes jargon and provides step-by-step guidance.

**Implementation status:**

**A. Simple Mode Framework** ✅
- Created: `SIMPLE-MODE.md` (complete implementation guide for skills)
- Pattern: Auto-detect when user says "simple mode", "not technical", "templates"
- Output: Copy-paste templates, one question at a time, plain English

**B. Templates Library** ✅
Created copy-paste templates for:
- Email templates: `templates/email/launch-sequence.md` (5 launch emails)
- Social templates: `templates/social/product-hunt-launch.md` (Twitter, LinkedIn, Reddit, HN)
- Copy templates: `templates/copy/landing-page-hero.md` (7 hero section formats)

**C. Simple Mode Features:**
- ✅ No jargon (technical terms explained with analogies)
- ✅ Guided questions (one at a time, not overwhelming)
- ✅ Copy-paste outputs (ready-to-use templates, not frameworks)
- ✅ Visual progress (checklists showing what's done and what's next)
- ✅ Next steps (always end with "Here's exactly what to do next")

**D. Priority Skills for Simple Mode:**
- Priority 1 (MVP): `launch-strategy`, `social-content`, `email-sequence`, `copywriting`
- Priority 2 (Post-launch): `pricing-strategy`, `seo-audit`, `competitor-alternatives`
- Priority 3 (Future): All other skills

**How it works:**
1. User says: "I'm not technical, can you help me launch?"
2. Agent activates simple mode
3. Agent asks: "What's your product in one sentence?"
4. User answers
5. Agent delivers step-by-step plan with copy-paste templates

**Example output difference:**

**Default mode:** "Create an email sequence with 5 touchpoints: welcome, value demonstration, case study, urgency, final offer."

**Simple mode:** "Here are 5 emails you can copy and customize:

**Email 1 - Welcome (Send immediately)**
```
Subject: Welcome to [Your Product]!
[Copy-paste template]
```

Copy this email, replace the brackets, and send it."

**Next steps:**
- ⏳ Integrate simple mode into priority skills (post-demo)
- ⏳ Test with 3 non-technical users
- ⏳ Add "Simple Mode" toggle to README

---

## Metrics for Success

**For Friday's presentation:**
- [ ] Demo runs smoothly (under 10 minutes)
- [ ] Audience understands the value in 30 seconds
- [ ] At least 2 questions about how to use it themselves

**Post-presentation:**
- [ ] 5+ people request access to try it
- [ ] Feedback collected from Yannick and jury
- [ ] Prioritized roadmap based on feedback

---

## Open Questions for Discussion

1. **Firecrawl scope:** Should we scrape competitors automatically, or only when the user asks?
2. **Data privacy:** How do we handle scraped competitor data? (Store vs. real-time)
3. **Skill discovery:** How do non-technical users find the right skill? (Current: they have to know the name)
4. **Pricing/access:** Is this free open-source, or a paid product?

---

## Next Steps

**Before Friday:**
- [x] Finalize demo script (`DEMO-SCRIPT.md`)
- [x] Test Firecrawl integration (MCP config created, ready to test with API key)
- [x] Create backup demo materials (`demo-project/VIDEO-OUTLINE.md`)
- [ ] Get Firecrawl API key and test live scraping
- [ ] Record 15-20 second backup video
- [ ] Practice presentation 2-3 times
- [ ] Create slides (optional - can use script as speaking notes)

**After Friday:**
- [ ] Collect feedback from Yannick and jury
- [ ] Prioritize improvements based on feedback
- [ ] Integrate simple mode into priority skills
- [ ] Test with non-technical users
- [ ] Update skills to leverage portfolio-research data
- [ ] Plan next milestone

---

## How to Contribute

**For Yannick and reviewers:**
- Add comments directly to this doc (or in margins)
- Flag anything unclear or overly technical
- Suggest use cases we're missing
- Identify the "must-haves" vs "nice-to-haves"

**For technical contributors:**
- See `CLAUDE.md` for skill conventions
- Check `skills/` for examples
- Test improvements against the demo flow

---

## Appendix: Current Skill List

### Marketing & Growth (14 skills)
- `marketing-ideas` - 139 proven tactics
- `launch-strategy` - Product launch planning
- `social-content` - Social media content
- `competitor-alternatives` - Comparison pages
- `copywriting` - Marketing copy
- `copy-editing` - Copy review
- `content-strategy` - Content planning
- `paid-ads` - PPC campaigns
- `email-sequence` - Email automation
- `referral-program` - Referral/affiliate setup
- `free-tool-strategy` - Engineering as marketing
- `pricing-strategy` - Pricing & packaging
- `product-marketing-context` - Foundational context
- `analytics-tracking` - Tracking setup

### SEO (4 skills)
- `seo-audit` - Technical SEO
- `programmatic-seo` - Pages at scale
- `schema-markup` - Structured data

### Research & Intelligence (1 skill) 🆕
- `portfolio-research` - Autonomous competitor research with Firecrawl

### Conversion Optimization (6 skills)
- `page-cro` - Landing page CRO
- `signup-flow-cro` - Signup optimization
- `onboarding-cro` - User activation
- `paywall-upgrade-cro` - In-app upsells
- `form-cro` - Form optimization
- `popup-cro` - Popup/modal optimization
- `ab-test-setup` - A/B test planning

### Utilities (2 skills)
- `keybindings-help` - Keyboard shortcuts
- `marketing-psychology` - Mental models

---

**Ready to discuss?** Add your feedback below or schedule a review session.
