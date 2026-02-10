# Friday Presentation Checklist

**Presentation date:** This Friday
**Time:** TBD
**Audience:** Startup accelerator class + jury
**Duration:** 8-10 minutes + Q&A

---

## ✅ Completed

- [x] Firecrawl MCP configuration created
- [x] `portfolio-research` skill built
- [x] Simple mode framework implemented
- [x] Templates library created (15+ templates)
- [x] Demo script written (word-for-word)
- [x] Sample project created (DevMetrics)
- [x] Video outline ready (15-20 seconds)
- [x] README updated
- [x] Roadmap document finalized
- [x] Setup guides written

---

## 🔥 Before Friday (High Priority)

### Day Before Presentation

- [ ] **Get Firecrawl API key**
  - Sign up at [firecrawl.dev](https://firecrawl.dev)
  - Copy API key
  - Add to `~/.claude/mcp-config.json`
  - Test with: `Research Notion and show me their pricing`

- [ ] **Practice presentation 2-3 times**
  - Run through demo script out loud
  - Time yourself (aim for 8-10 minutes)
  - Identify any stumbles or unclear parts
  - Practice Q&A responses

- [ ] **Test demo flow end-to-end**
  ```bash
  cd demo-project
  # Open in Claude Code
  # Run all demo commands:
  # 1. "Help me plan a launch strategy for DevMetrics"
  # 2. "Create social posts for my Product Hunt launch"
  # 3. "Research LinearB, Haystack, and Swarmia"
  ```

- [ ] **Prepare backup materials**
  - [ ] Screenshot each demo step
  - [ ] Save screenshots to `demo-project/demo-assets/screenshots/`
  - [ ] Test offline demo (internet fails scenario)

---

## 📹 Optional (If Time Permits)

- [ ] **Record 15-20 second video**
  - Follow `demo-project/VIDEO-OUTLINE.md`
  - Record screen showing:
    - Typing a command
    - Agent delivering results instantly
    - Firecrawl scraping competitors
  - Speed up to 1.5x-2x
  - Add text overlays
  - Export as MP4

- [ ] **Create slides**
  - Slide 1: Problem (founder pain point)
  - Slide 2: Solution (what is Habitat Skills)
  - Slide 3: Traction (25+ skills, demo)
  - Slide 4: Vision (Firecrawl, simple mode)
  - Optional: Can use `DEMO-SCRIPT.md` as speaking notes instead

---

## 🎯 Day of Presentation

### 30 Minutes Before

- [ ] **Tech setup**
  - [ ] Open `demo-project/` in Claude Code
  - [ ] Test internet connection
  - [ ] Close all other apps (minimize distractions)
  - [ ] Increase terminal font size (readable from back of room)
  - [ ] Turn off notifications (Do Not Disturb mode)

- [ ] **Verify demo works**
  - [ ] Run: `What's my product?` (should return DevMetrics)
  - [ ] Run: `Help me plan a launch strategy`
  - [ ] (If Firecrawl works) Run: `Research Notion`

- [ ] **Prepare backup**
  - [ ] Have screenshots folder open
  - [ ] Have backup video ready (if created)
  - [ ] Have `DEMO-SCRIPT.md` open in another window

- [ ] **Print materials (optional)**
  - [ ] One-pager with QR code to GitHub repo
  - [ ] Contact info for follow-up

### During Presentation

**Opening (30 seconds)**
- [ ] Hook: Start with founder pain point
- [ ] Transition: "Or... you use Habitat Skills"

**Demo 1: Launch Strategy (2 minutes)**
- [ ] Type: `Help me plan a launch strategy for my developer tool`
- [ ] Point out: No 20 questions, just results
- [ ] Highlight: Structured framework, not generic advice

**Demo 2: Chaining Skills (3 minutes)**
- [ ] Type: `Create social posts for my Product Hunt launch`
- [ ] Type: `Draft a launch email sequence`
- [ ] Point out: Skills work together like a marketing team

**Demo 3: Firecrawl (2 minutes)**
- [ ] Type: `Research Notion, Coda, and Airtable. Show me how to differentiate.`
- [ ] Show: Agent scraping websites
- [ ] Point out: 10 competitors analyzed in 30 seconds

**Closing (1 minute)**
- [ ] Summary: 26 skills, open source, built for founders
- [ ] Vision: Autonomous research, simple mode, more skills
- [ ] CTA: GitHub QR code, "Try it this weekend"

**Q&A**
- [ ] Refer to Q&A prep in `DEMO-SCRIPT.md`
- [ ] Have backup examples ready if asked

---

## 🚨 Backup Plans

### If Internet Fails
1. Show pre-recorded video (15-20 seconds)
2. Walk through screenshots in `demo-assets/`
3. Talk through the output (show script in `DEMO-SCRIPT.md`)

### If Firecrawl Demo Fails
1. Say: "We're adding autonomous research with Firecrawl..."
2. Show pre-recorded video or screenshot
3. Explain how it works conceptually

### If Terminal Freezes
1. Have backup terminal window open
2. Switch to screenshots
3. Continue presentation from slides

### If Wrong Output
1. Stay calm, say "Let me try that again"
2. Rephrase the command
3. If still wrong, switch to backup screenshot

---

## 📊 Post-Presentation

### Immediately After

- [ ] **Collect feedback**
  - [ ] Note questions that were asked
  - [ ] Note concerns or objections
  - [ ] Ask Yannick for feedback
  - [ ] Ask jury for feedback

- [ ] **Capture interest**
  - [ ] Share GitHub link in chat: `github.com/ycanerden/habitat-skills`
  - [ ] Collect email addresses from interested people
  - [ ] Invite them to try it this weekend

### Within 24 Hours

- [ ] **Follow-up email**
  - [ ] Send GitHub link
  - [ ] Include demo video (if created)
  - [ ] Share `WHATS-NEW.md` highlights
  - [ ] Invite feedback

- [ ] **Social media**
  - [ ] Post demo video on Twitter/LinkedIn
  - [ ] Tag Habitat, accelerator, and jury
  - [ ] Use hashtags: #HabitatSkills #OpenSource #Founders

### Within 1 Week

- [ ] **Implement feedback**
  - [ ] Review all notes from presentation
  - [ ] Prioritize top 2-3 improvements
  - [ ] Update `IMPROVEMENT-ROADMAP.md`
  - [ ] Create issues on GitHub for next steps

---

## 🎤 Presenter Tips

### Energy
- Start strong with the problem (founders know this pain)
- Show enthusiasm when demos work
- Stay calm if things break (backup plan ready)

### Pacing
- Speak slowly and clearly
- Pause after key points
- Don't rush through demos (let output appear)

### Engagement
- Make eye contact with audience
- Ask rhetorical questions ("Sound familiar?")
- Use "you" language ("Imagine you're launching...")

### Troubleshooting
- If demo fails: "No problem, let me show you this way..."
- If asked a tough question: "Great question. Let me think..."
- If running long: Skip Stage 3 (chaining demo)
- If running short: Add a backup example

---

## 🔗 Quick Links

**Demo materials:**
- [DEMO-SCRIPT.md](DEMO-SCRIPT.md) - Full presentation script
- [demo-project/](demo-project/) - Sample project
- [FIRECRAWL-SETUP.md](FIRECRAWL-SETUP.md) - Setup instructions

**Documentation:**
- [IMPROVEMENT-ROADMAP.md](IMPROVEMENT-ROADMAP.md) - Implementation status
- [WHATS-NEW.md](WHATS-NEW.md) - Feature summary
- [SIMPLE-MODE.md](SIMPLE-MODE.md) - Simple mode guide

**Templates:**
- [templates/email/](templates/email/) - Email templates
- [templates/social/](templates/social/) - Social media templates
- [templates/copy/](templates/copy/) - Landing page copy

---

## ✅ Final Check (Morning Of)

- [ ] Firecrawl working?
- [ ] Demo project loads?
- [ ] Internet stable?
- [ ] Backup materials ready?
- [ ] Confident with script?

**If all checked:** You're ready! 🚀

---

## 📞 Emergency Contacts

**During demo, if Claude breaks:**
- Restart Claude Code
- Switch to backup screenshots
- Show pre-recorded video

**After demo, for questions:**
- GitHub: github.com/ycanerden/habitat-skills/issues
- Habitat: joinhabitat.eu

---

**You've got this. Good luck! 🎉**
