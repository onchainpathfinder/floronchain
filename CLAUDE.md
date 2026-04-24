# CLAUDE.md — floronchain.com

> Read this file at the start of every session. Follow all rules below without being reminded.

---

## Site Identity

- **Site name:** FLOR🦩NCHAIN (the shared O between FLOR and ONCHAIN is rendered as a flamingo emoji 🦩)
- **Domain:** floronchain.com
- **Also lives as:** the ONCHAIN pillar on followtheflor.com
- **Hosting:** Netlify (project: theonchainpathfinder — legacy name, domain is floronchain.com)
- **Tech:** Static HTML site — single index.html deployed via Netlify
- **Tagline:** "Crypto compliance, without the corporate lawyer voice."
- **Purpose:** Crypto compliance, iGaming regulation, and AI/automation education for compliance professionals, crypto founders, and crypto beginners
- **Main goal:** Educational — teach, build authority, monetise expertise

---

## About the Author

**Floriana** — AML professional and crypto enthusiast since 2017.

Works at the intersection of financial crime prevention and digital asset innovation.

**Focus areas:** Compliance frameworks for crypto businesses, crypto crime investigation and typologies, onchain analysis, EU regulatory landscape, AML red flags in crypto transactions, AI & automation in regulated industries.

**Bio:** "AML professional, crypto enthusiast since 2017, writing about the intersection of compliance, crypto crime, and onchain analysis."

**IMPORTANT:** Never reference employer, company name, or full surname in public-facing content. Flor only.

---

## Audience (by monetisation priority)

1. **Compliance professionals** — MLROs, analysts, risk managers in crypto/iGaming. Want practical guidance, regulatory updates, red flag libraries. Will pay for deep guides and toolkits.
2. **Crypto founders & operators** — Building exchanges, DeFi protocols, payment platforms. Want "what do I need to do to be compliant?" in plain language. Will pay for readiness guides and consultation.
3. **Crypto-curious & degens** — Use crypto but don't understand the regulatory landscape. Want "what does this mean for ME?" Monetise through volume, newsletter growth, community.

---

## Content Categories

| Category | Slug | Topics |
|---|---|---|
| Crypto AML/CFT | `aml` | Red flags, typologies, transaction monitoring, suspicious activity, Chainalysis data |
| MiCA & EU Regulation | `mica` | Markets in Crypto-Assets, implementation timelines, requirements by entity type |
| iGaming Regulation | `igaming` | Gambling compliance, licensing, cross-border issues, sector-specific AML |
| Web3 Compliance | `web3` | DeFi, DAOs, NFTs, stablecoins from a regulatory lens |
| AI & Automation | `ai-automation` | AI in compliance, automation tools, how AI changes the compliance landscape |
| Regulation Explainers | `regulation` | New laws, consultations, enforcement actions, what they mean in practice |

---

## Content Formats

- **Long-form articles** (800-1500 words) — deep analysis, practical guidance
- **Quick explainers** (400-600 words) — single concept, "X explained in 5 minutes"
- **Red flag guides** — categorised indicators for specific typologies/sectors
- **Regulation breakdowns** — new regulation drops, what changed, who's affected, what to do
- **AI & automation pieces** — how AI/automation intersects with compliance

---

## Articles Published / In Progress

- Human trafficking and crypto typologies
- Deepfakes and crypto fraud
- Chainalysis 2026 Crypto Crime Report analysis
- FATF virtual assets guidance
- Crypto Crime in 2026: What Actually Matters
- Airdrops, DeFi opportunities and risks
- MiCA regulatory framework
- Bitcoin halving analysis
- Onchain analysis introduction
- Travel Rule compliance
- UAE FIU Virtual Asset Crime Report
- FATF Cyber-Enabled Fraud Report
- Crypto Trafficking Surge 2025

---

## Voice & Tone

- **Tone:** Professional and authoritative, but human. Not academic, not corporate. "Bloomberg meets crypto Twitter."
- **Audience:** Compliance officers trying to understand DeFi + crypto natives wanting regulatory clarity
- **Style:** Make complex topics accessible without dumbing them down. Lead with expertise, not lifestyle.
- **Perspective:** Real-world practitioner — not academic, not speculative
- **Italian/Maltese:** Use sparingly. An occasional "allura" is fine; this brand leans more international.
- **NEVER:** Corporate jargon without explanation, speculation presented as fact, generic takes, clickbait regulatory fear-mongering, content that could be mistaken for legal advice (always disclaim)
- **ALWAYS:** What it means in practice, who it affects, what to do about it, specific examples, Flor's honest take

---

## Distribution Channels (priority order)

1. **X/Twitter** (PRIMARY) — crypto compliance discourse lives here. Threads, single tweets with bold takes, quote-tweet regulatory news with analysis.
2. **Newsletter** (Beehiiv — planned) — educational series, links back to articles, builds owned audience.
3. **YouTube** (when ready) — explainer videos, 5-10 minutes, same structure as articles.
4. **LinkedIn** (OPTIONAL) — only for genuinely educational content. Professional tone, max 150 words, no personal branding energy. Use cautiously.

**NOT on Instagram** — this brand is not lifestyle content.

---

## Tools & Reports Referenced

**Onchain Analysis Tools:** Chainalysis Reactor, TRM Labs, Arkham Intelligence, Etherscan, Nansen

**Key Reports:** Chainalysis Crypto Crime Report (annual), FATF Virtual Assets Guidance, EU AML Package, Europol IOCTA, TRM Labs reports

**Regulatory Bodies:** FATF, EBA, AMLA, FinCEN, FCA, EU Commission (MiCA, AMLR/AMLD6)

---

## AML Risk Checker Tool

The site has a built-in AML Risk Checker tool (tools.html).
- Rule-based keyword scoring system (no API dependency)
- 16 AML red flag categories including mixers/tumblers, structuring, high-risk jurisdictions, wash trading, pig butchering indicators, rapid layering
- Output: Risk score + red flag explanations + compliance recommendations

---

## Design Spec

- **Dark theme** — pure black (`#000000`) background. Nightclub-meets-boardroom aesthetic.
- **Primary accent:** neon flamingo pink `#ff2db7` (with deeper pink `#ff006e` for pressed states)
- **Secondary accent:** neon cyan `#00f0ff` (for gradients, code highlights, info states)
- **Logo glow:** the 🦩 in FLOR🦩NCHAIN carries a neon pink drop-shadow (see `.claude/skills/floronchain-writer/references/brand-visual-system.md`)
- Fonts: Space Grotesk for headings, Plus Jakarta Sans for body (already wired in index.html)
- Cards with hover effects for article previews
- Mobile responsive
- Category filtering on articles page
- Sticky navigation: Home, Articles, About, Resources
- **NEVER revert to teal/green (#00d4aa, #00b894, #00ffa3).** Those were the retired "Onchain Pathfinder" palette.

---

## Deployment

- Site is a single index.html file
- Deploy by dragging folder into Netlify deploy zone
- Domain: floronchain.com (DNS pointed to Netlify)
- GitHub repo: github.com/onchainpathfinder/onchain-pathfinder (secondary)

---

## Monetisation Plan

- Phase 1: Affiliate links (Revolut, crypto tools, Booking.com)
- Phase 2: Digital products (compliance templates, red flag guides, jurisdiction checklists)
- Phase 3: Consulting pipeline — site as lead generation
- Newsletter: Beehiiv (planned)

---

## Legal Disclaimer

Every article must end with a variation of:
> *This content is for educational and informational purposes only. It does not constitute legal, financial, or compliance advice. Always consult a qualified professional for advice specific to your situation.*

Keep the wording natural — not identical every time. But it must always be there.

---

## Skills

- **floronchain-writer** — use in Cowork for writing articles, guides, red flag breakdowns, regulation explainers
- **mlro-aml-compliance** — use for creating compliance document templates (if creating products for sale)

---

## Core Rules

1. Every article must be accurate — compliance content has real-world consequences
2. Cite sources: link to FATF guidance, Chainalysis reports, official regulations
3. Never reference employer or full professional identity
4. Make complex topics accessible without dumbing them down
5. Separate brand: floronchain is PUBLIC education. Work documents go in AML-FDJ-United, never here.
6. Always search for current regulatory info before writing — laws change
7. Every article needs a keyword plan before drafting

---

## Folder Structure

```
floronchain/
├── CLAUDE.md              ← This file
├── .skills/               ← Installed skills
│   └── floronchain-writer/
├── index.html             ← Live site
├── tools.html             ← AML Risk Checker
├── content/               ← Article drafts and published content
│   ├── aml/
│   ├── mica/
│   ├── igaming/
│   ├── web3/
│   ├── ai-automation/
│   └── regulation/
└── references/            ← Source material, reports, regulation links
```
