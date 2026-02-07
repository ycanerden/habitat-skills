---
name: landing-page
version: 1.0.0
description: "Build a conversion-focused landing page — copy, structure, and code. Use when the user mentions 'landing page,' 'build a landing page,' 'homepage,' 'waitlist page,' 'coming soon page,' 'launch page,' or 'I need a website for my startup.' For copy improvements on an existing page, see related copywriting skills. For post-launch conversion optimization, see related CRO skills."
---

# Landing Page

You are helping a founder build a landing page that converts visitors into signups, waitlist members, or customers. This is often the first tangible thing a founder ships — make it count.

## Before Starting

**Check for context first:**
If `.claude/founder-context.md` exists, read it. Use the idea, audience, positioning, and competitive info to inform the page.

If no context exists, gather:
- What's the product? (one sentence)
- Who is it for?
- What should visitors do? (sign up, join waitlist, book a demo, buy)
- Do you have a brand/logo already?
- Any tech preference? (Framer, Next.js, HTML, Astro, etc.)

## Page Strategy

Before writing a single line of copy, decide:

### 1. Page Type

| Type | When to Use | Primary Action |
|------|------------|----------------|
| **Waitlist page** | Pre-product — testing demand | Email capture |
| **Launch page** | Product exists — driving signups | Sign up / Start free trial |
| **Sales page** | Selling a paid product | Purchase / Book demo |
| **Coming soon** | Building in public — teasing | Email capture + follow on social |

### 2. Traffic Source

Where are visitors coming from? This determines what they already know.

| Source | What They Know | Headline Approach |
|--------|---------------|-------------------|
| **Cold (ads, SEO)** | Nothing about you | Lead with problem/outcome |
| **Warm (social, referral)** | Heard of you, curious | Lead with differentiation |
| **Hot (direct, email)** | Know you, ready to act | Lead with CTA, reduce friction |

### 3. One-Page Argument

The page should build a single logical argument, top to bottom:

1. **Here's your problem** (hook them)
2. **Here's a better way** (introduce solution)
3. **Here's proof it works** (build credibility)
4. **Here's how to start** (call to action)

## Page Structure

### Above the Fold

**Headline**
Your single most important message. Rules:
- Communicate the core outcome or transformation
- Be specific — not "Build better products" but "Go from idea to prototype in one evening"
- Test these formulas:
  - `[Achieve outcome] without [pain point]`
  - `[Achieve outcome] in [timeframe]`
  - `Stop [unpleasant thing]. Start [desired thing].`
  - `The [category] for [specific audience]`
  - `[Outcome] — [how/qualifier]`

**Subheadline**
Expands on the headline. Adds specificity. 1-2 sentences max.
- If headline is outcome-focused → subheadline explains how
- If headline is problem-focused → subheadline introduces the solution

**Primary CTA**
- Action-oriented: "Start Free Trial" not "Sign Up"
- Communicate what they get: "Get Early Access" not "Submit"
- If waitlist: "Join the waitlist" or "Reserve your spot"
- Add a risk-reducer below the button: "Free for 14 days. No credit card needed."

**Hero visual** (optional but recommended)
- Screenshot of the product (if it exists)
- Mockup or prototype preview
- Illustration of the outcome
- Skip if you don't have something good — a clean text hero beats a bad image

### Social Proof Section

Place immediately after the hero if you have strong proof. Options:

| Proof Type | Minimum Needed | Example |
|-----------|---------------|---------|
| **Logos** | 3-5 recognizable names | "Trusted by teams at..." |
| **Numbers** | 1 impressive stat | "1,200+ startups launched" |
| **Testimonials** | 2-3 specific quotes | Quote + name + role + photo |
| **Press/media** | 2-3 logos | "Featured in..." |

**If you have no social proof yet:** Skip this section entirely. Don't fabricate it.

### Problem Section

Make the visitor feel understood. Show you know their pain.

- Describe the problem in their language (use verbatim customer words from founder-context)
- Show the cost of the status quo
- Agitate — what happens if they don't solve this?

**Format options:**
- 3 pain points with icons
- "Sound familiar?" followed by scenarios
- Before/after comparison

### Solution Section

Connect your product to their problem. Rules:
- **Benefits over features.** "Save 5 hours per week" not "Automated reporting engine"
- **Show, don't tell.** Screenshots, GIFs, or demo videos beat bullet points
- **3-5 key benefits max.** Don't list everything. Pick what matters most.

**Format options:**
- Feature cards with benefit-focused headlines
- Screenshot + text alternating left/right
- "How it works" 3-step process

### How It Works

Reduce perceived complexity. Show the path from signup to value.

**Format:** 3 steps (occasionally 4). Never more.

```
1. [First action] — [what happens / what they get]
2. [Second action] — [what happens / what they get]
3. [Third action] — [the outcome / transformation]
```

Keep descriptions to 1-2 sentences each.

### Testimonials / Social Proof (expanded)

If you have testimonials, place a fuller section here.

**Good testimonial formula:**
- Specific situation before
- What they did (used your product)
- Specific result after
- Name, role, company, photo

**Weak testimonials to avoid:**
- "Great product!" (vague)
- "Love it!" (no specifics)
- Anonymous quotes (not credible)

### Objection Handling

Address the top 3 reasons someone wouldn't sign up. Options:

- **FAQ section** — question-and-answer format
- **Comparison table** — you vs. alternatives
- **Risk reversals** — "Cancel anytime," "Free tier forever," "Money-back guarantee"

### Final CTA

Repeat the primary call to action. This is for people who scrolled the whole page and need one more nudge.

- Recap the core value in one sentence
- Repeat the CTA button
- Add urgency if appropriate (limited spots, launch date, early-access pricing)

## Copy Principles

### Clarity Over Cleverness
If you have to choose between clear and creative, choose clear.

### Specific Over Vague
- Bad: "Save time on your workflow"
- Good: "Cut your weekly reporting from 4 hours to 15 minutes"

### Customer Language
Use words your audience uses. If they say "find customers," don't write "acquire users."

### Active Voice
"We send your report every Monday" not "Reports are sent every Monday."

### Cut the Filler
Remove: "In order to," "It is important to note that," "At the end of the day," "Leverage," "Utilize," "Streamline," "Innovative."

## Technical Implementation

If the founder wants you to build the page (not just write copy):

### Tech Stack Recommendations

| Situation | Recommendation | Why |
|-----------|---------------|-----|
| **Fastest (no-code)** | Framer | Drag-and-drop, fast deploys, good templates |
| **Fastest (code)** | Single HTML file + Tailwind CDN | Zero build step, instant deploy |
| **Needs a waitlist** | HTML + Formspree / Buttondown / ConvertKit | Simple email capture |
| **Needs auth/app later** | Next.js + Vercel | Grows with the product |
| **Maximum simplicity** | Carrd | $19/year, dead simple |

### If Building in Code

Provide a complete, deployable file. Include:
- Responsive design (mobile-first)
- Semantic HTML
- Clean typography (Inter or system fonts)
- Proper meta tags (title, description, OG image)
- Email capture form (connected or with a placeholder endpoint)
- Minimal JS — no frameworks unless needed

### Deploy Recommendations

- **Vercel:** `vercel deploy` — free tier, instant
- **Netlify:** Drag-and-drop deploy — free tier
- **GitHub Pages:** Free, simple for static sites
- **Framer:** Built-in hosting

## Output Format

### 1. Page Copy

Organized by section:
```
[HERO]
Headline: ...
Subheadline: ...
CTA: ...

[SOCIAL PROOF]
...

[PROBLEM]
...

[SOLUTION]
...

[HOW IT WORKS]
...

[TESTIMONIALS]
...

[FAQ]
...

[FINAL CTA]
...
```

### 2. Annotations

For key decisions, explain why:
- "I led with [X] because your audience comes from [source] and already knows [Y]"
- "I chose a waitlist page over a signup page because you're pre-product"

### 3. Headline Alternatives

Provide 3 options with rationale:
- Option A: [copy] — [why]
- Option B: [copy] — [why]
- Option C: [copy] — [why]

### 4. Code (if requested)

Complete, deployable file(s) with everything included.

### 5. Meta Content

- Page title (50-60 chars)
- Meta description (150-160 chars)
- OG title and description

## Principles

- **Ship over perfect.** A live landing page with okay copy beats a perfect page that's never published. Help them get something live tonight.
- **One page, one action.** Every element should push toward the primary CTA. Remove anything that distracts.
- **Mobile-first.** Over 50% of traffic is mobile. Design for small screens first.
- **Speed matters.** No heavy images, no unnecessary JS. Fast pages convert better.
- **Honest copy only.** Never fabricate stats, testimonials, or social proof. If they don't have proof points, skip that section — don't fake it.

## Related Skills

- `founder-context` — Set up context before building
- `idea-validation` — Validate the idea the page is about
- `competitor-research` — Research competitors to differentiate positioning
- `mvp-scope` — Scope what gets built beyond the landing page
- `first-users` — Drive traffic to the landing page
