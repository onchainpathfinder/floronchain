---
name: infographic-builder
description: "Turns textual content into structured, visual-friendly infographic layouts suitable for reports, presentations, social media, and educational materials. Trigger on: 'infographic', 'visual summary', 'make this visual', 'turn this into an infographic', 'visual breakdown', 'one-pager visual', 'data snapshot', 'visual cheat sheet', 'process visual', 'visual explainer', or when the user provides dense text, steps, stats, or comparisons and wants them presented in a scannable, designed format. Also trigger when the user asks for a visual version of a report, policy, procedure, article, or any content that would benefit from being condensed into a single visual page. Do NOT use for flowcharts or system diagrams (use excalidraw-diagram-generator), data charts/graphs (use data-visualization), or full slide decks (use pptx)."
---

# Infographic Builder

You transform dense text, data, processes, and concepts into structured infographic layouts — scannable, visual-first formats that communicate key information at a glance.

## Core Philosophy

An infographic earns its existence by making information faster to absorb than reading the source text. If someone has to study the infographic as carefully as they'd study a paragraph, it hasn't done its job.

- **Scannable in 10 seconds** — the viewer should get the main takeaway at a glance
- **Visual hierarchy does the work** — size, colour, and position signal importance, not decoration
- **Less text, more structure** — if a section has more than 2 short sentences, it's too wordy
- **Data points over paragraphs** — pull out numbers, percentages, and key facts as standalone callouts
- **Consistent visual language** — icons, colours, and shapes mean the same thing throughout

## Workflow

### Step 1: Understand the content

Before designing anything, clarify:

| Question | Why it matters |
|---|---|
| **What's the source material?** (article, report, procedure, stats, comparison) | Determines infographic type |
| **Who's the audience?** (executives, team members, social followers, regulators) | Determines tone and detail level |
| **What's the single key takeaway?** | This drives the headline and visual emphasis |
| **Where will it be used?** (report insert, social post, presentation handout, internal doc) | Determines dimensions and format |

### Step 2: Choose the infographic type

| Type | Best for | Structure |
|---|---|---|
| **Statistical snapshot** | Data-heavy content, KPIs, survey results | Big numbers + short context lines |
| **Process / timeline** | Step-by-step procedures, chronologies | Numbered or connected stages |
| **Comparison** | Two or more options, before/after, pros/cons | Side-by-side columns or split layout |
| **List / checklist** | Tips, red flags, requirements, criteria | Icon + short text per item |
| **Hierarchy / pyramid** | Priority levels, risk tiers, categories | Layered sections, largest at base |
| **Hub and spoke** | Central concept with related sub-topics | Central element with radiating sections |
| **Anatomy / breakdown** | Explaining parts of a whole | Labelled sections of a central image or concept |

### Step 3: Extract and structure the content

Work through the source material and extract:

1. **Headline** — one punchy line that captures the whole infographic (max 8 words)
2. **Subtitle** — one sentence of context (optional)
3. **Key data points** — numbers, percentages, dates that deserve visual emphasis
4. **Sections** — group related information into 3–6 sections (more than 6 becomes cluttered)
5. **Section headings** — short, active labels (e.g., "What triggers an alert" not "Information regarding alert triggers")
6. **Bullet content** — max 1–2 lines per bullet, written as fragments not full sentences
7. **Callout** — one standout fact, quote, or stat that deserves a highlight box
8. **Source / footer** — attribution, date, disclaimers if needed

### Step 4: Define the visual layout

Produce a structured layout spec:

```
INFOGRAPHIC: [Title]
TYPE: [Statistical / Process / Comparison / List / Hierarchy / Hub-Spoke / Anatomy]
DIMENSIONS: [Portrait A4 / Landscape A4 / Square (social) / Custom]
AUDIENCE: [Who this is for]
COLOUR PALETTE: [Primary, Secondary, Accent — max 3–4 colours]

HEADER:
- Headline: "[Main title]"
- Subtitle: "[One-line context]"
- Visual: [icon/illustration suggestion]

SECTION 1: "[Section heading]"
- Layout: [icon-list / stat-callout / side-by-side / numbered-steps]
- Content:
  - [Item 1]
  - [Item 2]
  - [Item 3]
- Emphasis: [which item or stat to make visually dominant]

SECTION 2: "[Section heading]"
- Layout: [...]
- Content: [...]

[... repeat for each section ...]

CALLOUT BOX:
- Text: "[Standout stat or quote]"
- Style: [highlight colour, large font, bordered box]

FOOTER:
- Source: "[Attribution]"
- Date: "[When produced]"
- Branding: "[Logo / author if applicable]"
```

### Step 5: Produce the output

Depending on the user's needs, produce one of:

1. **Structured spec** (as above) — for the user to hand to a designer or build in Canva/Figma
2. **HTML infographic** — a single self-contained HTML file with inline CSS that renders the infographic visually. Use clean typography, colour blocks, icons (via emoji or SVG), and CSS grid/flexbox for layout. This is the default if the user wants something they can see immediately.
3. **Markdown visual** — a formatted markdown document that approximates the infographic layout using headers, callout blocks, tables, and emoji markers. Good for embedding in docs or Notion.

When producing HTML infographics:
- Use a fixed-width container (e.g., 800px) centred on the page
- Use Google Fonts or system fonts for clean typography
- Use CSS custom properties for the colour palette so it's easy to retheme
- Use emoji or simple SVG icons — don't rely on external icon libraries
- Include a print-friendly `@media print` section
- Make sure it looks good when saved as a PDF from the browser

## Quality Standards

**A great infographic:**
- Communicates the main message within 10 seconds of viewing
- Has no section with more than 3 short bullet points
- Uses colour purposefully (to group, highlight, or differentiate — never just to decorate)
- Has clear visual hierarchy — the most important thing is the biggest/boldest
- Works in black and white (colour adds meaning but isn't required to understand it)
- Fits on a single page or screen

**A failed infographic:**
- Is just a wall of text with coloured backgrounds
- Has more than 6 sections competing for attention
- Uses random icons that don't relate to the content
- Requires reading every word to understand the message
- Has inconsistent styling across sections

## Domain-Specific Patterns

### AML / Compliance infographics
- Use red/amber/green colour coding for risk levels
- Lead with the regulatory requirement or risk
- Include jurisdiction tags where relevant
- Keep language precise — compliance infographics are reference material, not marketing

### Content / Marketing infographics
- Lead with a hook or surprising stat
- Use brand colours if available
- Design for shareability — square format works best for social
- Include a clear CTA or takeaway at the bottom

### Educational / Explainer infographics
- Build from simple to complex (top to bottom)
- Use numbered steps or a clear flow
- Include a "key terms" or "remember" callout box
- Keep jargon minimal — if you must use it, define it inline

## Tips

- When in doubt, remove content rather than add it — infographics die from overcrowding
- Test readability by squinting at the layout — the structure should be visible even when blurry
- If a section needs a paragraph of text, it probably belongs in a report, not an infographic
- Pair every stat with a one-line "so what" — "42% increase" means nothing without "highest growth since 2019"
- Use contrast (dark on light, light on dark) to create visual sections without borders
