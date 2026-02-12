# BIOBUILDS Blog Content Engine — Instructions for Claude Code

## What This Repo Is

This is NOT a software project. This is the **blog content repository** for BIOBUILDS,
a Passivhaus-certified modular timber-frame home manufacturer operating in Romania,
Germany, and Austria. The repo contains blog articles in HTML format across three languages.

Your job: **Write one SEO-optimized blog post per day** that matches the existing
style, format, and quality standards.

---

## Company Context

**BIOBUILDS** builds Passivhaus-certified modular homes using 98% organic materials.

- **Core value proposition**: 21-day factory production, 90-95% energy savings
- **Markets**: Romania, Germany, Austria (EU average pricing often referenced)
- **Certifications**: Passivhaus Classic/Plus/Premium
- **Partners**: Zehnder (MVHR), Pro Clima (airtightness), STEICO (insulation)
- **Price point**: €2,200/m² for certified Passivhaus (competitive vs market €2,700-3,500/m²)

The blog drives organic search traffic across 4 content pillars to generate leads
for the main biobuilds.com website.

---

## Repository Structure

```
/
├── EN/                          # English articles (16 files)
├── DE/                          # German articles (16 files)
├── RO/                          # Romanian articles (16 files)
├── blog-styles.css              # Unified CSS (252 lines, use ONLY these classes)
├── SEO.md                       # Keyword strategy + content rules (READ FIRST)
├── SOURCES.md                   # 200+ verified reference links (READ SECOND)
└── CLAUDE.md                    # This file
```

---

## The 4 Content Pillars

| Pillar | Code | Target Keywords | Language Focus |
|--------|------|-----------------|----------------|
| **Passivhaus** | 1.x | energy efficiency, certification, costs, savings | DE, EN |
| **Modular Construction** | 2.x | 21-day build, factory precision, vs traditional | EN, DE |
| **Timber-Frame** | 3.x | sustainability, CLT, health, LCA | EN, DE |
| **Prefab Homes** | 4.x | speed, simplicity, price, myths | RO, EN |

---

## Required Reading Order (Every Run)

1. **SEO.md** — Understand keyword targets, content structure rules, E-E-A-T requirements
2. **SOURCES.md** — Your research database; every statistic must trace here
3. **Existing articles** — Read 2-3 from your target pillar to match style exactly
4. **blog-styles.css** — Use ONLY existing CSS classes; never invent new ones

---

## File Naming Convention

Format: `{Pillar}.{SubArticle} {LANG} {url-slug}.html`

Examples:
- `1.0 EN what-is-passive-house.html`
- `2.1 DE modular-vs-traditional-construction-full-comparison.html`
- `4.3 RO how-long-does-it-take-build-prefab-home.html`

Rules:
- Pillar number: 1 = Passivhaus, 2 = Modular, 3 = Timber-Frame, 4 = Prefab
- Sub-article: Sequential within pillar (0, 1, 2, 3...)
- Language: EN, DE, or RO
- Slug: lowercase, hyphens, descriptive

---

## How to Pick a Topic

1. **Count articles per pillar** in the language you're writing for
2. **Pick the pillar with the FEWEST articles** (balance coverage)
3. **Check SEO.md** for uncovered keywords in that pillar
4. **Verify no existing article covers this exact topic** (never duplicate)
5. **Confirm sufficient source material** in SOURCES.md

---

## Research Protocol

### Source Hierarchy (cite in this order of preference)

1. **Passive House Institute (PHI)** — passivehouse.com, passipedia.org
2. **Peer-reviewed journals** — Frontiers, ScienceDirect, MDPI, Springer
3. **EU/Government sources** — EPBD, EUR-Lex, national energy agencies
4. **Industry reports** — McKinsey, MBI, World Economic Forum
5. **BIOBUILDS pages** — biobuilds.com (for internal links)
6. **Wikipedia** — For foundational definitions (GEO visibility boost)

### Research Steps

1. Pick 3-5 relevant sources from SOURCES.md
2. Use **WebFetch** to read those pages and extract real data
3. Use **WebSearch** for 1-2 fresh sources (2025-2026 data)
4. Cross-reference statistics across multiple sources
5. Never cite a number you can't trace to a source
6. **BIOBUILDS fact-check pass**: Before finalizing the article, use **WebFetch** on the relevant biobuilds.com pages to verify every claim you make about BIOBUILDS (pricing, timelines, materials, certifications, specs). If the site doesn't confirm it, remove it.

---

## Writing Rules

### Structure (Match Existing Articles)

1. **Full HTML5 document** with `<!DOCTYPE html>`, `<head>`, `<body>`
2. **Meta tags**: title, description, Open Graph, Twitter Card
3. **Schema.org markup** (JSON-LD in `<head>`):
   - Article, BreadcrumbList, FAQPage, Organization, Person
4. **Hero section** with image, breadcrumb, category, title, author meta
5. **TL;DR box** (50-70 words, answers primary query)
6. **Table of Contents** with smooth-scroll anchors
7. **Body content** with H2/H3 hierarchy, stats boxes, blockquotes
8. **FAQ section** with accordion (3-5 questions)
9. **Author card** with credentials
10. **CTA box** linking to biobuilds.com/design or /savings
11. **Related articles** section (2-3 internal links)
12. **Share buttons** (LinkedIn, Facebook, copy link)

### Tone

- **Professional but approachable** — not academic, not salesy
- **Data-driven** — every claim backed by a source
- **Answer-first** — lead each section with the direct answer
- **Confident expertise** — "We've certified over 400 units"
- **Natural BIOBUILDS tie-back** — when connecting the topic to BIOBUILDS, make it feel organic and welcome; the reader should think "oh, these guys actually do this" — not "this is an ad"; weave BIOBUILDS in where the topic genuinely calls for a real-world example, a practical solution, or a next step — never shoehorn it in

### Length

- **2,000-3,000 words** body content (match existing articles)
- **50-70 words** TL;DR
- **40-60 words** per featured snippet paragraph
- **100-300 words** per extractable passage

### Language Matching

- **EN articles**: Write in English
- **DE articles**: Write in German
- **RO articles**: Write in Romanian
- Match the exact tone, phrasing patterns, and formality level of existing articles in that language

---

## CSS Classes (Use ONLY These)

All classes use the `bb-` prefix. Reference `blog-styles.css` for the full list.

**Layout:**
- `.bb-hero`, `.bb-hero-image`, `.bb-hero-overlay`, `.bb-hero-content`
- `.bb-container`, `.bb-article`, `.bb-body`

**Typography:**
- `.bb-hero-title`, `.bb-hero-category`, `.bb-hero-breadcrumb`

**Components:**
- `.bb-tldr`, `.bb-tldr-content`
- `.bb-toc`, `.bb-toc-list`, `.bb-toc-link`
- `.bb-stat`, `.bb-stat-number`, `.bb-stat-label`
- `.bb-stats-row`, `.bb-stat-cell`
- `.bb-takeaway`
- `.bb-comparison` (for tables)
- `.bb-faq`, `.bb-faq-item`, `.bb-faq-question`, `.bb-faq-answer`
- `.bb-author`, `.bb-author-card`, `.bb-author-avatar`
- `.bb-cta`, `.bb-cta-title`, `.bb-cta-btn`
- `.bb-related`, `.bb-related-grid`, `.bb-related-card`
- `.bb-share`, `.bb-share-btn`

**Never invent new CSS classes.** If you need styling not covered, use existing classes creatively.

---

## Schema Markup Template

```json
{
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "Article",
      "@id": "https://biobuilds.com/blog/[slug]#article",
      "headline": "[Title]",
      "description": "[Meta description]",
      "datePublished": "[YYYY-MM-DD]",
      "dateModified": "[YYYY-MM-DD]",
      "author": {
        "@type": "Person",
        "name": "Andreea B.",
        "jobTitle": "Client Experience Lead",
        "description": "Passive House Consultant with 8 years experience"
      },
      "publisher": {
        "@type": "Organization",
        "@id": "https://biobuilds.com#organization"
      },
      "inLanguage": "[en|de|ro]",
      "articleSection": "[Guides|Analysis|Comparison]"
    },
    {
      "@type": "BreadcrumbList",
      "itemListElement": [
        {"@type": "ListItem", "position": 1, "name": "Home", "item": "https://biobuilds.com"},
        {"@type": "ListItem", "position": 2, "name": "Blog", "item": "https://biobuilds.com/blog"},
        {"@type": "ListItem", "position": 3, "name": "[Article Title]"}
      ]
    },
    {
      "@type": "FAQPage",
      "mainEntity": [
        {
          "@type": "Question",
          "name": "[Question text matching H2/H3 exactly]",
          "acceptedAnswer": {
            "@type": "Answer",
            "text": "[Direct answer, 50-100 words]"
          }
        }
      ]
    },
    {
      "@type": "Organization",
      "@id": "https://biobuilds.com#organization",
      "name": "BIOBUILDS",
      "url": "https://biobuilds.com",
      "logo": "https://cdn.prod.website-files.com/6801f60a2febd7da21a30b43/6801f6c304852fb7ed2291d0_Biobuilds%20Logo%20Modular%203.0.avif"
    }
  ]
}
```

---

## Hard Rules (Never Break These)

1. **NEVER run git commands** — no git add, commit, push, branch, checkout
2. **NEVER create pull requests** — the workflow handles this
3. **NEVER invent statistics** — every number traces to a source
4. **NEVER use CSS classes that don't exist** in blog-styles.css
5. **NEVER duplicate a topic** already covered by an existing article
6. **NEVER use placeholder images** — use real BIOBUILDS CDN URLs from existing articles
7. **NEVER write in the wrong language** — match the target directory (EN/DE/RO)
8. **ALWAYS tie back to BIOBUILDS — naturally** — every article must connect to BIOBUILDS (biobuilds.com) and their passive homes/products by the conclusion, but the tie-back must feel **natural and welcome**, not forced or salesy; weave BIOBUILDS into the narrative where it genuinely fits the topic so the reader sees it as a helpful recommendation, not an ad
9. **TRIPLE-CHECK every BIOBUILDS claim** — before stating anything about BIOBUILDS homes, pricing, specs, certifications, timelines, or capabilities as fact, use **WebFetch** to verify it against the live biobuilds.com website (check relevant pages: /design, /efficient, /healthy, /prefabricated, /projects, and the homepage); if you cannot confirm a claim on their actual site, **do not include it** — no hallucinated company data, ever

---

## Error Handling

If any of these conditions occur, **describe the problem clearly and STOP**:

- SEO.md or SOURCES.md is missing or empty
- Cannot determine the correct blog directory structure
- Cannot read existing articles to match format
- No uncovered topics remain in the target pillar
- Research sources are insufficient for the chosen topic
- blog-styles.css is missing or unreadable

Do NOT guess or improvise. Report the issue so a human can fix it.

---

## Example Workflow

1. Read SEO.md → understand keyword strategy
2. Read SOURCES.md → identify research material
3. Count: EN/ has 4 Passivhaus, 4 Modular, 3 Timber-Frame, 4 Prefab
4. Decision: Write Timber-Frame (Pillar 3) article in English
5. Read `3.0 EN timber-frame-safety-sustainability.html` to match format
6. Read blog-styles.css to confirm available classes
7. Research: WebFetch 3 sources from SOURCES.md, WebSearch for 2025 data
8. Write: `3.3 EN [new-topic].html` matching exact format
9. **BIOBUILDS verification**: WebFetch biobuilds.com pages to triple-check every BIOBUILDS-specific claim in the article — remove or correct anything the site doesn't confirm
10. Ensure the article ties back to BIOBUILDS and their passive homes/products
11. Save file to `/EN/` directory
12. STOP — workflow handles commit, push, PR

---

## Author Information

Use this author for all articles:

- **Name**: Andreea B.
- **Title**: Client Experience Lead
- **Credentials**: Certified Passive House Consultant, 8 years experience
- **Avatar**: Use existing avatar URL from other articles

---

## Internal Links (Use These)

When linking to BIOBUILDS pages:

- **Configurator**: https://biobuilds.com/design
- **Savings Calculator**: https://biobuilds.com/savings
- **Projects Gallery**: https://biobuilds.com/projects
- **Efficiency Page**: https://biobuilds.com/efficient
- **Health Page**: https://biobuilds.com/healthy
- **Prefab Page**: https://biobuilds.com/prefabricated

For related articles, link to other posts in the same language directory.

---

## Success Criteria

A successful article:

- [ ] Matches existing file format exactly
- [ ] Uses correct filename convention
- [ ] Saved in correct language directory (EN/, DE/, or RO/)
- [ ] Contains complete Schema.org markup
- [ ] Has 6-10 cited sources per 1,000 words
- [ ] Includes TL;DR, TOC, FAQ, Author, CTA, Related sections
- [ ] Uses only existing CSS classes
- [ ] Targets an uncovered keyword from SEO.md
- [ ] Contains no invented statistics
- [ ] Written in the correct language
- [ ] Article ties back to BIOBUILDS and their passive homes/products
- [ ] All BIOBUILDS-specific claims verified against live biobuilds.com pages via WebFetch
