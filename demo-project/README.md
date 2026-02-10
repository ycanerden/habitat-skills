# Demo Project for Habitat Skills

This directory contains everything you need for the Friday presentation demo.

## Contents

- `.claude/founder-context.md` - Pre-filled product context for DevMetrics (demo product)
- `VIDEO-OUTLINE.md` - Shot list and script for 15-20 second backup video
- `demo-assets/` - Screenshots, slides, and backup materials

## Setup Instructions

### Before the Presentation

1. **Open this directory in Claude Code:**
   ```bash
   cd demo-project
   code .  # or your preferred editor
   ```

2. **Verify founder context loads:**
   ```
   # In Claude Code, type:
   What's my product?

   # Should respond with DevMetrics details
   ```

3. **Test Firecrawl (if using):**
   ```
   # In Claude Code, type:
   Research Notion and show me their pricing

   # Should scrape notion.so and return pricing info
   ```

4. **Prepare backup screenshots:**
   - Take screenshots of each demo step
   - Save in `demo-assets/screenshots/`
   - In case internet fails during live demo

## Demo Flow

### Demo 1: Launch Strategy (2 minutes)
**Type in Claude Code:**
```
Help me plan a launch strategy for DevMetrics
```

**Expected output:**
- Pre-launch checklist
- Launch day playbook (Product Hunt, Twitter, email)
- Post-launch tactics

### Demo 2: Social Content (1 minute)
**Type in Claude Code:**
```
Create social posts for my Product Hunt launch
```

**Expected output:**
- Twitter launch thread
- LinkedIn announcement
- Product Hunt tagline

### Demo 3: Portfolio Research (2 minutes)
**Type in Claude Code:**
```
Research LinearB, Haystack, and Swarmia. How should I differentiate?
```

**Expected output:**
- Competitor profiles (positioning, pricing, features)
- Market insights
- Differentiation recommendations

## Backup Materials

### If Internet Fails
1. Use pre-recorded video (15-20 seconds)
2. Or use screenshots in `demo-assets/screenshots/`
3. Or use slide deck in `demo-assets/slides/`

### If Firecrawl Fails
- Fall back to web search instead of scraping
- Or use pre-written example output in `demo-assets/portfolio-research-example.md`

## Product Context (DevMetrics)

**Elevator pitch:**
"Real-time analytics for GitHub repositories. Helps engineering managers track PR velocity, code review time, and team productivity. Set up in 30 seconds."

**Key differentiators:**
- Fastest setup (vs LinearB's complex onboarding)
- Built for small teams (vs enterprise-focused tools)
- Affordable ($29/mo vs $50-200/mo)

**Target audience:**
Engineering managers at startups (10-50 person teams)

**Stage:**
MVP with 50 beta users, launching publicly in 2 weeks

## Questions to Prepare For

**Q: How is this different from ChatGPT?**
A: Structured frameworks vs generic advice. Skills chain together like a marketing team.

**Q: Can non-technical founders use it?**
A: We're adding "simple mode" with copy-paste templates and no jargon.

**Q: What's the business model?**
A: Open source now. Exploring freemium, SaaS, or marketplace models.

**Q: How does Firecrawl work?**
A: Web scraping API via Model Context Protocol. Autonomous competitor research.

## Post-Demo Actions

- [ ] Share GitHub link: github.com/canerden/habitat-skills
- [ ] Collect email addresses from interested people
- [ ] Note all feedback and questions
- [ ] Send follow-up email with demo video

## Troubleshooting

**Issue: Founder context doesn't load**
- Check file exists: `.claude/founder-context.md`
- Restart Claude Code
- Manually paste context into chat

**Issue: Skills not triggering**
- Use explicit skill names: "Use the launch-strategy skill"
- Or rephrase: "Help me plan a launch" → triggers launch-strategy

**Issue: Firecrawl not working**
- Check MCP config: `~/.claude/mcp-config.json`
- Verify API key is set
- Fall back to manual research

---

**Ready for Friday! 🚀**
