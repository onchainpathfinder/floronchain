---
name: floronchain-writer
description: "Writes educational crypto compliance, iGaming regulation, and AI/automation content for floronchain.com (and the ONCHAIN pillar of followtheflor.com). Use this skill whenever Flor says: 'write a floronchain article', 'onchain article about [topic]', 'MiCA explainer', 'write about crypto AML', 'red flag guide for [typology]', 'regulation breakdown', 'AI in compliance article', 'iGaming regulation piece', 'crypto compliance content', 'floronchain post about [topic]', or anything about writing published educational content on crypto regulation, AML, MiCA, iGaming compliance, or AI/automation in regulated industries. Also activate when given regulatory news or a compliance topic and asked to produce an article or explainer. Do NOT use for internal compliance documents (use mlro-aml-compliance instead), Instagram captions, or followtheflor lifestyle/running/explores content (use followtheflor-article-writer instead)."
---

## Overview

This skill produces publish-ready educational content for floronchain.com — Flor's expert brand covering crypto compliance, iGaming regulation, and AI/automation in regulated industries.

The key difference from other Flor skills:
- **followtheflor-article-writer** = lifestyle content (running, Malta, personal brand)
- **mlro-aml-compliance** = internal compliance documents (policies, procedures, training decks)
- **floronchain-writer** (this skill) = published educational content that builds Flor's authority as a crypto compliance expert

Before writing anything, read:
- `references/brand-visual-system.md` for the FlorOnChain colour palette, fonts, and React component specs
- `references/interactive-tools-guide.md` when building interactive tools or apps for the blog

---

## Workflow

### Step 1: Identify the content format

Ask if not clear from context:

- **Long-form article** (800-1500 words) — the default. Deep analysis, practical guidance.
- **Quick explainer** (400-600 words) — single concept, no tangents. "X explained in 5 minutes."
- **Red flag guide** — categorised indicators for a specific typology or sector. Heavy on tables.
- **Regulation breakdown** — when new regulation drops. What changed, who's affected, what to do.
- **AI & automation piece** — how AI/automation intersects with compliance, crypto, iGaming.

### Step 2: Identify the audience

The content should work for multiple audiences, but knowing the primary target shapes the depth and tone:

- **Compliance professionals** → can handle technical terms, want practical application, cite specific legislation
- **Crypto founders** → need plain language, want "what do I need to do", focus on business impact
- **Beginners** → no assumed knowledge, define everything, use analogies
- **All** → layer the content: accessible surface, depth for those who want it

### Step 3: Keyword plan BEFORE writing

This is non-negotiable — same rule as followtheflor.

Identify:
- One primary keyword (what someone would search to find this)
- 2-5 secondary keywords
- Search intent: informational / commercial / transactional
- Category: mica / aml / igaming / web3 / ai-automation / regulation

Confirm the plan makes sense before proceeding. If the topic is too vague, ask Flor to narrow it.

### Step 4: Research what's ranking

Search for the top content on this topic. For crypto compliance content specifically, look at:
- What regulatory bodies have published (ESMA, FIAU, EBA — primary sources matter here)
- What compliance blogs and publications cover it (Elliptic, Chainalysis blog, ACAMS)
- What's missing — often the "what does this actually mean in practice" angle is underserved
- Reddit/X discussions — what questions are real people asking about this regulation?

The goal: produce something more useful, more practical, and more clearly written than what's already out there. If you can't beat the top 3 results, rethink the angle.

### Step 5: Draft the article

**Voice — the critical difference from followtheflor:**

floronchain content leads with expertise, not lifestyle. Flor is still present — it's her analysis, her perspective, her experience — but the reader comes for the knowledge, not the personality. Think of it as the difference between a friend telling you about their run (followtheflor) and a friend who happens to be a compliance expert explaining what MiCA means for your crypto startup (floronchain).

**Writing rules:**

- Clear, direct sentences. No filler.
- Explain complex concepts without oversimplifying — respect the reader's intelligence
- Every claim backed by a source or specific regulation reference
- Use "in practice, this means..." to bridge from regulation text to real-world impact
- Tables for structured information (red flags, timelines, requirements by entity type)
- Short paragraphs (2-4 sentences max)
- H2 subheadings that tell the reader what each section delivers
- The reader should be able to scan H2s and get 80% of the value

**What makes floronchain content stand out:**

1. **The "so what" factor** — never just summarise a regulation. Always answer: what does this mean for you?
2. **Practical examples** — "If you're running a crypto exchange in Malta, this means you need to..."
3. **Flor's take** — a brief, honest opinion section. "Here's what I think this means for the industry." This is where Flor's personality comes through most.
4. **Timeliness** — if writing about regulation, include dates, deadlines, transition periods
5. **Cross-references** — link between crypto, iGaming, and AI/automation where they intersect (they often do)

**Structure by content format:**

**Long-form article:**
```
Hook (2-3 lines — question, bold claim, or news peg)
Context (why this matters right now)
The substance (3-4 H2 sections — the actual analysis)
Flor's take (1-2 paragraphs — honest opinion)
What to do about it (actionable next steps)
CTA (question that invites discussion)
Disclaimer
```

**Quick explainer:**
```
What is [concept]? (2-3 paragraphs)
Why it matters (1-2 paragraphs)
What happens next (1 paragraph)
Disclaimer
```

**Red flag guide:**
```
Overview of the typology/sector
Red flags by category (tables — customer, transaction, geographic, product, channel)
Real-world scenario (fictitious data, clearly disclaimed)
What to do if you spot these flags
Disclaimer
```

**Regulation breakdown:**
```
What changed (1-2 paragraphs — the news)
Who's affected (specific entity types, jurisdictions)
Timeline (key dates in a table)
What you need to do now (actionable steps by audience)
Flor's take
Disclaimer
```

**AI & automation piece:**
```
The problem (what's inefficient/broken in compliance today)
How AI/automation addresses it (specific tools, workflows, approaches)
Limitations and risks (be honest — AI in compliance has real limitations)
Practical implementation (how to actually start using this)
Flor's take
Disclaimer
```

### Step 6: Format as MDX

Output the complete article in MDX format with correct frontmatter:

```mdx
---
title: "Article Title Here"
description: "140-160 char meta description with CTA"
date: "YYYY-MM-DD"
pillar: "onchain"
category: "mica" | "aml" | "igaming" | "web3" | "ai-automation" | "regulation"
tags: ["tag1", "tag2", "tag3"]
primaryKeyword: "main keyword"
readingTime: "X min read"
audience: "compliance" | "founders" | "beginners" | "all"
---
```

Save to: `content/onchain/`

### Step 7: Generate distribution content

After the article, produce companion content for each channel:

**X/Twitter thread (5-8 tweets):**
```
Tweet 1: [HOOK] — bold claim, surprising stat, or provocative question. Must stop the scroll.
Tweet 2-6: Key points from the article. One idea per tweet. No thread-padding.
Tweet 7: Flor's take — the opinion that makes people quote-tweet.
Tweet 8: CTA — "Full breakdown: [link]" or "More in my newsletter: [link]"
```

**Newsletter snippet (for Beehiiv):**
```
Subject line: [compelling, specific, under 50 chars]
Preview text: [first line that appears in inbox]

Body: 2-3 paragraphs. One key insight from the article.
End with link to the full piece.
```

**YouTube script (when applicable — skip if the topic is too text-dependent):**
```
[HOOK — first 10 seconds]
Bold statement or question that frames the topic.

[CONTEXT — 60 seconds]
Why this matters right now. Set up the problem.

[SUBSTANCE — 3-6 minutes]
The core analysis. Use "imagine you're running a crypto exchange..." to make it concrete.

[FLOR'S TAKE — 30-60 seconds]
Honest opinion. This is where personality shines.

[CTA — 10 seconds]
Subscribe, newsletter, link in description.
```

**LinkedIn (OPTIONAL — only include if Flor requests it):**
Professional, educational tone only. Max 150 words. No personal branding energy.

---

## Output Format

Deliver in this order:
1. **Keyword plan** (5 lines max)
2. **Full MDX article** (saved to content/onchain/)
3. **X/Twitter thread**
4. **Newsletter snippet**
5. **YouTube script** (if applicable)
6. **LinkedIn post** (only if requested)

---

## Quality Standard

A perfect output:
- Teaches something specific — the reader leaves knowing more than when they arrived
- Has a clear "so what" — not just information, but interpretation and practical guidance
- Sounds like an expert who respects your time, not a textbook or a blog farm
- References specific legislation, dates, and entity types — not vague generalities
- Includes Flor's honest take — the opinion that makes the content feel human
- Passes the "would a compliance officer bookmark this?" test
- SEO fundamentals in place: keyword in title, first 100 words, one H2, meta description
- Ends with a disclaimer

A failed output:
- Reads like a Wikipedia summary of a regulation
- Could have been written by anyone with access to Google
- Uses "it depends" without explaining what it depends on
- Has no practical guidance — just description
- Is fear-mongering or sensationalist about regulation
- Missing the disclaimer
- Over 1500 words with no reason to be

---

## Edge Cases

**Flor provides regulatory news ("write about this new ESMA consultation"):**
Do a regulation breakdown. Research the actual consultation document before writing.

**Topic overlaps with mlro-aml-compliance ("write about EDD procedures"):**
Ask: "Is this for publishing on floronchain (educational article for an audience) or for internal compliance use (a procedures document)?" Use the answer to pick the right skill.

**Topic is pure AI/automation with no compliance angle:**
Check with Flor. If there's no compliance, crypto, or iGaming connection, it might belong on followtheflor instead, or might not be on-brand at all.

**Topic is too broad ("write about MiCA"):**
Narrow it. "MiCA" → "MiCA requirements for crypto exchanges" or "MiCA stablecoin rules explained" or "MiCA implementation timeline 2025-2026".

**Topic requires legal specificity Flor can't verify:**
Flag it clearly. "This section references [specific regulation] — you should verify the current text before publishing, as regulations can be amended."

**Request for content that could be mistaken for legal advice:**
The disclaimer is mandatory, but also frame the content carefully. "Here's what the regulation says and what it generally means" rather than "Here's what you should do."

---

## References

Read `../followtheflor-article-writer/references/brand-context.md` before writing any content. It contains the full brand voice guide, audience segments, content format details, distribution channel rules, and SEO requirements.
