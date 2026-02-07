# Getting Started with Habitat Skills

A step-by-step guide for non-technical founders. No coding experience needed.

---

## What are Habitat Skills?

Habitat Skills are like cheat sheets for AI. When you install them, your AI assistant (Claude) learns how to help you with startup-specific tasks — validating ideas, researching competitors, building landing pages, and more.

Think of it like hiring a startup advisor that lives inside your terminal.

---

## What You Need

1. **A computer** (Mac, Windows, or Linux)
2. **Claude Code** installed (free to start)
3. **10 minutes** to set up

That's it. No coding required.

---

## Step 1: Install Claude Code

Claude Code is a terminal-based AI assistant made by Anthropic. Here's how to get it:

### On Mac

Open the **Terminal** app (search for "Terminal" in Spotlight — press Cmd + Space and type "Terminal").

Then paste this and press Enter:

```
npm install -g @anthropic-ai/claude-code
```

**Don't have npm?** You need Node.js first. Go to [nodejs.org](https://nodejs.org), download the installer, run it, then try the command above again.

### First time?

After installing, run:

```
claude
```

It will ask you to log in with your Anthropic account. Follow the prompts. Once you see the Claude prompt (`>`), you're in.

---

## Step 2: Create Your Project Folder

In Terminal, type:

```
mkdir my-startup && cd my-startup
```

This creates a folder called "my-startup" and moves you into it. You can name it whatever you want.

---

## Step 3: Install Habitat Skills

Still in Terminal, paste this:

```
git clone https://github.com/joinhabitat/habitat-skills.git .claude/skills/habitat
```

This downloads all the Habitat Skills into your project. Done.

---

## Step 4: Start Using the Skills

Launch Claude Code inside your project:

```
claude
```

Now you can talk to Claude and it knows all the Habitat frameworks. Here's what to try:

### Set Up Your Context (Do This First)

Type:

```
Help me set up my founder context
```

Claude will ask you about your idea, your audience, and your goals. Answer conversationally — it's like chatting with a co-founder. This saves your info so every other skill knows your situation.

### Validate Your Idea

```
Validate my startup idea
```

Claude will run your idea through a structured framework — problem severity, market size, riskiest assumptions — and give you a scorecard with next steps.

### Research Competitors

```
Research my competitors
```

Claude will search for competitors, analyze their strengths and weaknesses, and help you find your positioning angle.

### Build a Landing Page

```
Build me a landing page
```

Claude will write the copy AND the code for a landing page you can deploy tonight.

### Scope Your MVP

```
What should my MVP include?
```

Claude will help you cut your feature list down to the absolute minimum that tests your core idea.

### Find Your First Users

```
How do I find my first users?
```

Claude will create a playbook with specific outreach templates, channels, and a daily routine.

### Plan Your Launch

```
Help me plan my launch
```

Claude will build a phased launch strategy — what to do before, during, and after launch day.

---

## The Habitat Evening Workflow

If you're at a Habitat evening, here's the recommended order:

| Time | What to Do | Command |
|------|-----------|---------|
| **6:00 PM** | Set up your context | "Help me set up my founder context" |
| **6:15 PM** | Quick validation | "Validate my startup idea" |
| **6:30 PM** | Scope what to build tonight | "Scope my MVP for tonight" |
| **6:45 PM** | Start building | "Build me a landing page" or "Help me prototype this" |
| **9:30 PM** | Polish and ship | "Help me deploy this" |
| **10:00 PM** | Plan next steps | "How do I find my first users?" |

---

## Common Questions

### "I don't know how to use the terminal"

That's okay. Here's the absolute basics:

- **Open Terminal:** On Mac, press Cmd + Space, type "Terminal", press Enter
- **Type a command and press Enter** to run it
- **Copy-paste works:** Cmd + V to paste into Terminal
- That's all you need. Claude does the rest.

### "I don't have an idea yet"

Start with:

```
I don't have a specific idea yet. Help me brainstorm based on problems I've experienced.
```

Claude will walk you through it.

### "I tried a command and got an error"

Paste the error message to Claude:

```
I got this error: [paste the error here]. What do I do?
```

Claude can usually fix it for you.

### "Can I use this without Claude Code?"

The skills are markdown files — they work with any AI coding tool that supports them (Cursor, Codex, etc.). But Claude Code is the easiest way to get started.

### "Do I need to pay for anything?"

- **Claude Code:** Has a free tier. The Pro plan ($20/month) gives you more usage.
- **Habitat Skills:** Free and open source, forever.

---

## Quick Reference Card

Save this for the evening:

| I want to... | Say this to Claude |
|--------------|-------------------|
| Set up my project | "Help me set up my founder context" |
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
- **Found a bug or have a suggestion?** [Open an issue](https://github.com/joinhabitat/habitat-skills/issues) on GitHub.

Happy building.
