# Firecrawl Setup Guide

Enable autonomous competitor research in Habitat Skills using Firecrawl.

---

## What is Firecrawl?

Firecrawl is a web scraping API that lets AI agents automatically visit websites, extract content, and analyze data. With Firecrawl, the `portfolio-research` skill can:

- Scrape competitor websites (homepage, pricing, features)
- Extract positioning, pricing models, and target audiences
- Analyze 10+ competitors in seconds
- Provide actionable differentiation recommendations

---

## Setup (5 minutes)

### Step 1: Get a Firecrawl API Key

1. Go to [firecrawl.dev](https://firecrawl.dev)
2. Sign up for a free account
3. Copy your API key

**Free tier:**
- 500 credits/month
- ~50 page scrapes
- Perfect for testing

---

### Step 2: Configure MCP Server

The MCP (Model Context Protocol) configuration file has already been created at:
```
~/.claude/mcp-config.json
```

**Update the API key:**

```bash
# Open the config file
nano ~/.claude/mcp-config.json

# Replace YOUR_API_KEY_HERE with your actual key
{
  "mcpServers": {
    "firecrawl": {
      "command": "npx",
      "args": ["-y", "firecrawl-mcp"],
      "env": {
        "FIRECRAWL_API_KEY": "fc-your-actual-key-here"
      }
    }
  }
}
```

**Save and exit:**
- Press `Ctrl + O` (save)
- Press `Enter` (confirm)
- Press `Ctrl + X` (exit)

---

### Step 3: Restart Claude Code

Close and reopen Claude Code to load the new MCP configuration.

---

### Step 4: Test It

In Claude Code, type:

```
Research Notion and show me their pricing
```

**Expected behavior:**
- Agent uses Firecrawl to scrape notion.so
- Extracts pricing information
- Returns structured data

**If it works:** You'll see Firecrawl scraping status messages and pricing data.

**If it doesn't work:** See troubleshooting below.

---

## Usage Examples

### Example 1: Single Competitor
```
Research Notion and tell me how to differentiate
```

**Agent will:**
1. Scrape notion.so (homepage, pricing, features)
2. Extract positioning and pricing
3. Recommend differentiation angles

---

### Example 2: Multiple Competitors
```
Research Notion, Coda, and Airtable. Show me pricing and positioning.
```

**Agent will:**
1. Scrape all three websites
2. Create comparison table
3. Identify pricing clusters and messaging patterns

---

### Example 3: Use with Other Skills
```
Use portfolio-research to analyze my competitors, then use competitor-alternatives to create a comparison page
```

**Agent will:**
1. Scrape competitors using Firecrawl
2. Generate structured comparison page
3. Include features, pricing, and differentiators

---

## Troubleshooting

### Issue: "Firecrawl MCP not configured"

**Solution:**
1. Check that `~/.claude/mcp-config.json` exists
2. Verify API key is correct (starts with `fc-`)
3. Restart Claude Code

---

### Issue: "API key invalid"

**Solution:**
1. Log in to [firecrawl.dev](https://firecrawl.dev)
2. Copy a fresh API key
3. Update `~/.claude/mcp-config.json`
4. Restart Claude Code

---

### Issue: "Rate limit exceeded"

**Solution:**
- Free tier: 500 credits/month (~50 pages)
- If you hit the limit, upgrade to a paid plan
- Or wait until next month for credits to reset

---

### Issue: Scraping fails for specific site

**Solution:**
- Some sites block scrapers (rare)
- Try a different competitor
- Or fall back to manual research

---

## Without Firecrawl

If you don't have Firecrawl configured, the `portfolio-research` skill will:

1. Offer to help you set it up (with this guide)
2. Or fall back to web search (limited depth)
3. Or guide you through manual research

**Skills still work without Firecrawl—they just won't scrape automatically.**

---

## Cost & Limits

### Free Tier
- 500 credits/month
- ~50 page scrapes
- Good for: Testing, small-scale research

### Paid Plans
- Starts at $20/month
- 5,000+ credits
- Good for: Regular competitor research

**Recommendation:** Start with free tier. Upgrade if you need more.

---

## Privacy & Data

**What Firecrawl sees:**
- Public website content only
- No login-required pages
- No private data

**What's stored:**
- Nothing by default (real-time scraping)
- Firecrawl logs requests for debugging

**Best practices:**
- Only scrape public competitor sites
- Don't scrape personal or private data
- Respect robots.txt

---

## Advanced: Custom Scraping

The `portfolio-research` skill scrapes these pages by default:
1. Homepage (positioning, hero headline)
2. Pricing page (pricing model, tiers)
3. Features/product page (key features)
4. About page (target audience, company stage)

**Want to customize?** Edit `skills/portfolio-research/SKILL.md` and adjust the scraping strategy.

---

## FAQ

**Q: Is Firecrawl required for Habitat Skills?**
A: No. Most skills work without it. Only `portfolio-research` requires it for autonomous scraping.

**Q: Can I use a different scraping tool?**
A: Yes, but you'd need to modify the `portfolio-research` skill to use a different API.

**Q: Does this work for non-SaaS competitors?**
A: Yes, as long as they have a public website. Works for e-commerce, marketplaces, agencies, etc.

**Q: Can I scrape LinkedIn or private pages?**
A: No. Firecrawl only scrapes public, non-authenticated pages.

**Q: How accurate is the extracted data?**
A: Very accurate for well-structured sites. May need manual verification for complex sites.

---

## Next Steps

1. ✅ Set up Firecrawl (if you haven't already)
2. Test with `portfolio-research` skill
3. Use it to analyze competitors before your launch
4. Integrate insights into `competitor-alternatives` pages

**Need help?** Open an issue on GitHub or ask in the Habitat community.

---

## Resources

- [Firecrawl Documentation](https://docs.firecrawl.dev)
- [Firecrawl MCP Server](https://github.com/firecrawl/firecrawl-mcp-server)
- [Model Context Protocol](https://modelcontextprotocol.io)

---

**Happy researching! 🔥**
