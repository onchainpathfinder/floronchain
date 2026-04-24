# FLOR🦩NCHAIN — Visual Brand System

Use these specs when creating React components, infographics, title cards, or any visual assets for floronchain.com.

**Brand name display:** `FLOR🦩NCHAIN` — the shared O between FLOR and ONCHAIN is rendered as the flamingo emoji (🦩 / U+1F9A9). Never spell it "Floronchain" or "FlorOnChain" in display contexts.

## Colour Palette

| Token | Hex | Usage |
|-------|-----|-------|
| Background (main) | `#000000` | Page background — pure black |
| Background (secondary) | `#0a0a0a` | Section shifts |
| Background (cards) | `#141414` | Card surfaces |
| Background (card hover) | `#1f1f1f` | Card hover state |
| Accent (neon pink) | `#ff2db7` | CTAs, highlights, links, logo glow |
| Accent (deep pink) | `#ff006e` | Pressed/hover, emphasis |
| Accent (cyan) | `#00f0ff` | Secondary accent, gradients, code highlights |
| Accent glow | `rgba(255,45,183,0.55)` | Logo drop-shadow, neon glow |
| Text (primary) | `#f5f5f5` | Body text |
| Text (secondary) | `#a0aec0` | Captions, labels |
| Text (muted) | `#6b7280` | Footnotes, metadata |
| Border | `#1f1f1f` | Card/section borders |
| Danger/red | `#ef4444` | Alerts, red flags |
| Warning/amber | `#f59e0b` | Caution indicators |
| Info | `#00f0ff` | Informational elements (cyan instead of blue) |

## Typography

- **Headings + code:** `JetBrains Mono`
- **Body text:** `Inter`

## Spacing & Radius

- Card border radius: `14-16px`
- Button border radius: `8-10px`
- Card padding: `24px`
- Section gap: `32px`

## Logo

🦩 (flamingo emoji) — replaces the shared O in FLOR🦩NCHAIN. Always rendered with a subtle neon-pink drop-shadow glow:

```css
.logo-o {
  display: inline-block;
  filter: drop-shadow(0 0 6px rgba(255, 45, 183, 0.55));
  transition: filter 0.3s ease;
}
.logo:hover .logo-o {
  filter: drop-shadow(0 0 10px rgba(255, 45, 183, 0.9))
          drop-shadow(0 0 16px rgba(0, 240, 255, 0.35));
}
```

## React Implementation

```jsx
const COLORS = {
  bg: '#000000',
  bgSecondary: '#0a0a0a',
  card: '#141414',
  cardHover: '#1f1f1f',
  accent: '#ff2db7',
  accentDeep: '#ff006e',
  accentCyan: '#00f0ff',
  accentGlow: 'rgba(255,45,183,0.55)',
  text: '#f5f5f5',
  textSecondary: '#a0aec0',
  textMuted: '#6b7280',
  border: '#1f1f1f',
  danger: '#ef4444',
  warning: '#f59e0b',
  info: '#00f0ff',
};

const Logo = () => (
  <span className="logo">
    FLOR<span className="logo-o">🦩</span>NCHAIN
  </span>
);
```

## Design Principles

- Dark theme always — no light mode
- Subtle hover effects with accent glow
- `fadeIn` animations on card mount
- Card-based layouts
- Mobile-responsive: use `flexWrap: "wrap"` and `minWidth` patterns
- Inline React styles (no CSS classes) for self-contained components
