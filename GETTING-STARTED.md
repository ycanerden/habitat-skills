# Getting Started with Habitat Skills

A step-by-step guide for non-technical founders. No coding experience needed.

---

## What are Habitat Skills?

Habitat Skills are like cheat sheets for AI. When you install them, your AI assistant learns how to help you with startup-specific tasks — validating ideas, researching competitors, building landing pages, and more.

Think of it like hiring a startup advisor that lives inside your computer.

---

## What You Need

1. **A computer** (Mac, Windows, or Linux)
2. **An AI tool** (see options below)
3. **10 minutes** to set up

That's it. No coding required.

---

## Choose Your Tool

Habitat Skills work with multiple AI tools. Pick the one that fits you best:

| Tool | Cost | Best For | Setup |
|------|------|----------|-------|
| **Claude Code** | Pro $20/month | Best skills experience | Terminal |
| **Gemini CLI** | Free | Free terminal option | Terminal |
| **Cursor** | Free tier available | People who prefer an IDE | IDE |
| **Google Antigravity** | Free | Free IDE, no API key needed | IDE |
| **Google AI Studio** | Free | No install needed | Browser |
| **Claude.ai / ChatGPT** | Free tiers available | No install needed | Browser |

**Not sure?** Here's the simple guide:
- **Have a terminal and want the best experience?** → Claude Code
- **Have a terminal and want free?** → Gemini CLI
- **Prefer a code editor (IDE)?** → Cursor or Antigravity
- **Don't want to install anything?** → Google AI Studio, Claude.ai, or ChatGPT

### At a Habitat Evening?

Your organizer will share an API key at the start. You just need to:

1. Open Terminal (Cmd + Space → type "Terminal")
2. Paste the setup command you'll receive at the event
3. Start building

Skip to [Step 2](#step-2-create-your-project-folder) if your setup is provided at the event.

---

## Terminal Options

### Option A: Claude Code (Recommended)

The best experience. Skills activate automatically when you ask questions.

**Install:**

Open **Terminal** (Cmd + Space → type "Terminal" → press Enter).

```
npm install -g @anthropic-ai/claude-code
```

**Don't have npm?** Go to [nodejs.org](https://nodejs.org), download the installer, run it, then try again.

**First time?** Run `claude` and follow the login prompts. Once you see the Claude prompt, you're in.

Then continue to [Step 2](#step-2-create-your-project-folder).

---

### Option B: Gemini CLI (Free)

Google's free terminal AI. Uses the same skills format as Claude Code — no changes needed.

**Install:**

```
npm install -g @google/gemini-cli
```

**Don't have npm?** Go to [nodejs.org](https://nodejs.org), download the installer, run it, then try again.

**First time?** Run `gemini` and sign in with your Google account. Free tier gives you 60 requests/minute and 1,000/day — more than enough for an evening.

**Install skills:**

After creating your project folder ([Step 2](#step-2-create-your-project-folder)), clone the skills:

```
git clone https://github.com/ycanerden/habitat-skills.git .gemini/skills/habitat
```

Then run `gemini` in your project folder and type "Get started."

---

## IDE Options

### Option C: Cursor (Free Tier Available)

Cursor is a code editor with built-in AI. It has a generous free tier.

**Install:**

1. Download from [cursor.com](https://cursor.com)
2. Install and open it
3. Create your project folder and open it in Cursor

**Add the skills:**

In Cursor's terminal (View → Terminal), paste:

```
git clone https://github.com/ycanerden/habitat-skills.git .cursor/skills/habitat
```

**Use the skills:**

Open Cursor's AI chat (Cmd + L) and type naturally:

```
Get started
```

Cursor reads the skill files and follows the frameworks automatically.

---

### Option D: Google Antigravity (Free)

Google's free code editor (VS Code fork) with built-in Gemini AI. No API key needed — just sign in with Google.

**Install:**

1. Download from [developers.google.com/gemini/antigravity](https://developers.google.com/gemini/antigravity)
2. Install and open it
3. Create your project folder and open it in Antigravity

**Add the skills:**

Open the terminal in Antigravity (View → Terminal), paste:

```
git clone https://github.com/ycanerden/habitat-skills.git .gemini/skills/habitat
```

**Use the skills:**

Open the AI chat panel and type:

```
Get started
```

It works just like Cursor but uses Gemini (free) instead of Claude/GPT.

---

## Browser Options (No Install Needed)

### Option E: Google AI Studio (Easiest + Free)

1. Go to [aistudio.google.com](https://aistudio.google.com)
2. Sign in with your Google account
3. Start a new chat
4. Copy a skill file from the [quick links below](#quick-links-to-skill-files)
5. Paste it into the chat and say:

```
Use this framework to help me. Here's my idea: [describe your idea]

[paste the skill content here]
```

Free. No install. Works right now.

---

### Option F: Claude.ai or ChatGPT (No Install Needed)

Use the skills manually in any AI chat — no terminal required.

1. Go to [claude.ai](https://claude.ai) or [chatgpt.com](https://chatgpt.com)
2. Open a skill from the quick links below
3. Copy the full content of the skill file
4. Paste it into your chat with your idea:

```
Use the following framework to help me. Here's my idea: [describe your idea]

[paste the skill content here]
```

### Quick Links to Skill Files

- [Onboarding](https://github.com/ycanerden/habitat-skills/blob/main/skills/onboarding/SKILL.md) — Start here
- [Founder Context](https://github.com/ycanerden/habitat-skills/blob/main/skills/founder-context/SKILL.md)
- [Idea Validation](https://github.com/ycanerden/habitat-skills/blob/main/skills/idea-validation/SKILL.md)
- [Competitor Research](https://github.com/ycanerden/habitat-skills/blob/main/skills/competitor-research/SKILL.md)
- [Customer Segments](https://github.com/ycanerden/habitat-skills/blob/main/skills/customer-segments/SKILL.md)
- [Landing Page](https://github.com/ycanerden/habitat-skills/blob/main/skills/landing-page/SKILL.md)
- [MVP Scope](https://github.com/ycanerden/habitat-skills/blob/main/skills/mvp-scope/SKILL.md)
- [Prototype Sprint](https://github.com/ycanerden/habitat-skills/blob/main/skills/prototype-sprint/SKILL.md)
- [Pitch Deck](https://github.com/ycanerden/habitat-skills/blob/main/skills/pitch-deck/SKILL.md)
- [First Users](https://github.com/ycanerden/habitat-skills/blob/main/skills/first-users/SKILL.md)
- [Launch Plan](https://github.com/ycanerden/habitat-skills/blob/main/skills/launch-plan/SKILL.md)
- [Social Content](https://github.com/ycanerden/habitat-skills/blob/main/skills/social-content/SKILL.md)

**Tip:** Bookmark these links for quick access during the evening.

---

## Step 2: Create Your Project Folder

In Terminal, type:

```
mkdir my-startup && cd my-startup
```

This creates a folder called "my-startup" and moves you into it. Name it whatever you want.

---

## Step 3: Install Habitat Skills

Still in Terminal, paste the command for your tool:

**Claude Code:**
```
git clone https://github.com/ycanerden/habitat-skills.git .claude/skills/habitat
```

**Gemini CLI or Antigravity:**
```
git clone https://github.com/ycanerden/habitat-skills.git .gemini/skills/habitat
```

**Cursor:**
```
git clone https://github.com/ycanerden/habitat-skills.git .cursor/skills/habitat
```

This downloads all the Habitat Skills into your project. Done.

---

## Step 4: Start Using the Skills

Launch your AI tool inside your project:

| Tool | Command |
|------|---------|
| Claude Code | `claude` |
| Gemini CLI | `gemini` |
| Cursor | Open folder in Cursor → Cmd + L |
| Antigravity | Open folder in Antigravity → open AI chat |

Now you can talk to it and it knows all the Habitat frameworks. Here's what to try:

### Get Started (Do This First)

```
Get started
```

The onboarding skill will welcome you, ask for your idea in one sentence, and immediately show you what it can do. It takes under 2 minutes and sets up everything for the other skills.

### Validate Your Idea

```
Validate my startup idea
```

Runs your idea through a structured framework — problem severity, market size, riskiest assumptions — and gives you a scorecard with next steps.

### Research Competitors

```
Research my competitors
```

Searches for competitors, analyzes their strengths and weaknesses, and helps you find your positioning angle.

### Build a Landing Page

```
Build me a landing page
```

Writes the copy AND the code for a landing page you can deploy tonight.

### Scope Your MVP

```
What should my MVP include?
```

Cuts your feature list down to the absolute minimum that tests your core idea.

### Find Your First Users

```
How do I find my first users?
```

Creates a playbook with specific outreach templates, channels, and a daily routine.

### Plan Your Launch

```
Help me plan my launch
```

Builds a phased launch strategy — what to do before, during, and after launch day.

---

## The Habitat Evening Workflow

If you're at a Habitat evening, here's the recommended order:

| Time | What to Do | Say This |
|------|-----------|----------|
| **6:00 PM** | Get started | "Get started" |
| **6:15 PM** | Quick validation | "Validate my startup idea" |
| **6:30 PM** | Scope what to build tonight | "Scope my MVP for tonight" |
| **6:45 PM** | Start building | "Build me a landing page" or "Help me prototype this" |
| **9:30 PM** | Polish and ship | "Help me deploy this" |
| **10:00 PM** | Plan next steps | "How do I find my first users?" |

---

## Common Questions

### "I don't know how to use the terminal"

That's okay. Three options:

1. **The basics:** Open Terminal (Cmd + Space → "Terminal"), type a command, press Enter. Copy-paste works (Cmd + V). That's all you need.
2. **Use an IDE instead:** Try [Cursor](#option-c-cursor-free-tier-available) or [Antigravity](#option-d-google-antigravity-free) — they're visual code editors with AI built in.
3. **Skip everything:** Use [Google AI Studio](#option-e-google-ai-studio-easiest--free), [Claude.ai or ChatGPT](#option-f-claudeai-or-chatgpt-no-install-needed) — just copy skill content into an AI chat in your browser.

### "I don't have an idea yet"

Start with:

```
I don't have a specific idea yet. Help me brainstorm based on problems I've experienced.
```

The AI will walk you through it.

### "I tried a command and got an error"

Paste the error message to your AI tool:

```
I got this error: [paste the error here]. What do I do?
```

It can usually fix it for you.

### "Do I need to pay for anything?"

- **Habitat Skills:** Free and open source, forever.
- **At a Habitat evening:** Access is provided — you don't need to pay for anything.
- **On your own:** Gemini CLI, Google AI Studio, and Antigravity are free. Claude.ai and ChatGPT have free tiers. Claude Code is $20/month. Cursor has a free tier.

---

## Quick Reference Card

Save this for the evening:

| I want to... | Say this |
|--------------|---------|
| Set up my project | "Get started" |
| Test my idea | "Validate my startup idea" |
| Research competitors | "Research my competitors" |
| Decide what to build | "Scope my MVP" |
| Build a landing page | "Build me a landing page" |
| Build a prototype | "Help me prototype this in 5 hours" |
| Find users | "How do I find my first users?" |
| Plan a launch | "Help me plan my launch" |
| Get unstuck | "I'm stuck on [describe the problem]" |

---

## Need Help?

- **At a Habitat evening?** Raise your hand — mentors are here to help.
- **Building on your own?** Ask in the Habitat community or open an issue on GitHub.
- **Found a bug or have a suggestion?** [Open an issue](https://github.com/ycanerden/habitat-skills/issues) on GitHub.

Happy building.
