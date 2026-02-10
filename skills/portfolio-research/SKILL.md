---
name: portfolio-research
description: Autonomous research on portfolio companies, competitors, and market positioning using web scraping. Analyzes competitor websites to extract positioning, features, pricing, and target audience.
---

# Portfolio Research Skill

**When to use:** When the user mentions analyzing competitors, researching portfolio companies, understanding market positioning, or needs competitive intelligence.

**Related skills:**
- `competitor-alternatives` - Creates comparison pages after research
- `market-research` - Broader market analysis
- `product-marketing-context` - Stores foundational product context

---

## Skill Flow

### 1. Understand research scope

Ask clarifying questions if needed:
- "Which companies should I research?"
- "What specific information are you looking for?" (positioning, pricing, features, etc.)
- "Is this for competitive analysis, partnership research, or something else?"

### 2. Autonomous scraping with Firecrawl

**IMPORTANT:** This skill requires the Firecrawl MCP server to be configured. If not available, inform the user and fall back to manual research.

For each company:
1. Use Firecrawl to scrape their homepage and key pages (pricing, about, features)
2. Extract structured data:
   - **Positioning statement** - How they describe themselves (hero headline, tagline)
   - **Target audience** - Who they serve (job titles, company size, industry)
   - **Key features** - Top 5-10 features highlighted
   - **Pricing model** - Free trial, freemium, pricing tiers, starting price
   - **Social proof** - Customer logos, testimonials, case studies
   - **Differentiators** - What makes them unique (from their messaging)

3. Identify patterns:
   - Common messaging themes
   - Pricing clusters (e.g., most competitors charge $20-50/user/mo)
   - Feature gaps (what they all have vs. what's missing)

### 3. Synthesize findings

Create a structured report:

**A. Executive Summary**
- Key takeaways in 3-5 bullets
- Biggest opportunities (gaps in the market)
- Biggest threats (strong competitors)

**B. Company Profiles**
For each competitor, provide:
- **Name & URL**
- **One-line positioning**
- **Target audience**
- **Pricing** (starting price or model)
- **Standout features** (what they emphasize)
- **Positioning angle** (all-in-one, easiest, most powerful, etc.)

**C. Market Insights**
- **Common features** - Table stakes you must have
- **Pricing insights** - Where should you price?
- **Messaging patterns** - What language resonates?
- **White space opportunities** - Underserved segments or use cases

**D. Recommended actions**
- How to differentiate based on this research
- Which competitor(s) to position against
- Messaging angles to explore

---

## Example Interaction

**User:** "Research Notion, Coda, and Airtable to help me position my product"

**Agent:**
*[Uses Firecrawl to scrape notion.so, coda.io, airtable.com]*

**Portfolio Research: Notion, Coda, Airtable**

**Executive Summary**
- All three position as "all-in-one workspaces" but target different audiences
- Notion leads with simplicity, Coda with customization, Airtable with data/spreadsheets
- Pricing clusters around $10-20/user/month for team plans
- **Opportunity:** All are complex for non-technical users—simpler onboarding could be a differentiator
- **Threat:** Notion has strongest brand and network effects

**Company Profiles**

**Notion**
- URL: notion.so
- Positioning: "One workspace. Every team."
- Target: Knowledge workers, small teams, creators
- Pricing: Free plan + $10/user/mo (Plus), $18/user/mo (Business)
- Standout features: Databases, templates, AI assistant, collaborative docs
- Positioning angle: Simplicity + flexibility ("Write, plan, organize")

**Coda**
- URL: coda.io
- Positioning: "Docs that work like apps"
- Target: Product teams, operations, technical users
- Pricing: Free plan + $12/user/mo (Pro), $36/user/mo (Team)
- Standout features: Packs (integrations), automations, interactive tables
- Positioning angle: Power + customization ("Build anything")

**Airtable**
- URL: airtable.com
- Positioning: "Build powerful work apps, without code"
- Target: Operations teams, project managers, SMBs
- Pricing: Free plan + $20/user/mo (Team), $45/user/mo (Business)
- Standout features: Spreadsheet-database hybrid, views, forms, automations
- Positioning angle: Data-first ("Connected apps for any workflow")

**Market Insights**

**Common features (table stakes):**
- Real-time collaboration
- Templates
- Mobile apps
- Integrations
- Free tier

**Pricing insights:**
- Free tiers are generous (to drive network effects)
- Team pricing: $10-20/user/mo
- Enterprise: $18-45/user/mo
- All offer annual discounts (15-20%)

**Messaging patterns:**
- Lead with "all-in-one" or "flexibility"
- Emphasize collaboration and team use cases
- Use verbs: "Build," "Organize," "Connect"
- Social proof on homepage (customer logos)

**White space opportunities:**
- **Simpler onboarding** - All have steep learning curves
- **Vertical-specific** - None are tailored for specific industries
- **Lightweight use cases** - Overkill for simple task management
- **Better mobile experience** - All are desktop-first

**Recommended Actions**

1. **Positioning approach:**
   - If simpler: "Like Notion, but you'll be productive in 5 minutes"
   - If vertical: "[Your Industry]'s all-in-one workspace"
   - If focused: "Just [specific use case], done right"

2. **Primary competitor to position against:**
   - Notion (if targeting knowledge workers and teams)
   - Airtable (if emphasizing data/operations)
   - Coda (if targeting power users)

3. **Messaging angles to test:**
   - "No learning curve" (vs. their complexity)
   - "Purpose-built for [X]" (vs. their generality)
   - "Faster to value" (vs. their feature bloat)

---

**Next steps:**
- Use `competitor-alternatives` to create comparison pages
- Update `product-marketing-context` with these insights
- Run `copywriting` to draft positioning based on differentiation

---

## Fallback (No Firecrawl)

If Firecrawl MCP is not configured, offer manual research:

"I don't have web scraping enabled yet. I can still help in two ways:

1. **You provide URLs** - Share the competitor websites and I'll guide you on what to look for
2. **I'll use web search** - I can search for publicly available info (limited depth)

Want to set up Firecrawl for autonomous research? It takes 2 minutes:
1. Get a free API key from firecrawl.dev
2. Add this to `~/.claude/mcp-config.json`:

```json
{
  "mcpServers": {
    "firecrawl": {
      "command": "npx",
      "args": ["-y", "firecrawl-mcp"],
      "env": {
        "FIRECRAWL_API_KEY": "your_key_here"
      }
    }
  }
}
```

Then I can scrape and analyze competitors automatically."

---

## Notes for Non-Technical Users

**What this skill does in plain English:**

Instead of manually visiting competitor websites and taking notes, this skill:
1. Automatically visits their website
2. Reads their homepage, pricing page, and features
3. Extracts: what they say they do, who they target, how much they charge
4. Summarizes it all in a structured report

**Why this matters:**
- Saves hours of manual research
- Helps you find gaps in the market (what no one else is doing)
- Informs your pricing and positioning decisions
- Gives you data to back up your strategy

**Limitations:**
- Only scrapes public information (no login-required content)
- Won't analyze product UX (just marketing messaging)
- Best for SaaS/software competitors with public websites

---

## Technical Notes

**MCP server requirements:**
- Firecrawl MCP server: `npx -y firecrawl-mcp`
- Requires `FIRECRAWL_API_KEY` environment variable
- Free tier: 500 credits/month (~50 page scrapes)

**Scraping strategy:**
1. Homepage (positioning, hero headline)
2. Pricing page (pricing model, tiers)
3. Features/product page (key features)
4. About page (target audience, company stage)

**Data extraction approach:**
- Use Firecrawl's structured extraction
- Fallback to keyword/pattern matching if needed
- Store results in markdown tables for readability

**Rate limiting:**
- Scrape sequentially (1 company at a time)
- Wait 2-3 seconds between page requests
- Respect robots.txt

---

## Version History

- **v1.0** (Feb 2026) - Initial release with Firecrawl integration
