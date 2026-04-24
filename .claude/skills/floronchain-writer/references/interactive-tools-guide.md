# FlorOnChain — Interactive Tools & Apps Guide

The blog features interactive React-based tools that readers can use. These drive engagement, demonstrate expertise, and build trust toward consulting services.

## Tool Types

- **Risk assessment tools** — Transaction risk scorers, compliance readiness checkers, jurisdiction risk comparators
- **Educational quizzes** — AML regulation knowledge tests, red flag identification challenges
- **Lookup/reference tools** — Regulation finders, sanctions regime comparators, FATF recommendation guides
- **Calculators** — Threshold calculators, risk scoring tools, compliance cost estimators

## Technical Requirements

- Self-contained React functional components with hooks
- Use the `COLORS` object from `brand-visual-system.md` for all styling
- Inline React styles (no CSS classes)
- `JetBrains Mono` for headings, `Inter` for body
- Card-based layouts, `borderRadius: 14-16`, subtle hover effects, `fadeIn` animations
- Mobile-responsive: `flexWrap: "wrap"`, `minWidth` patterns

## Mandatory Disclaimer

Every tool must include:
```
⚠️ This tool is for educational purposes only and does not constitute legal or compliance advice.
```

## AI-Powered vs Local Tools

- For tools needing dynamic analysis → use the Anthropic API pattern from existing implementations
- For static logic tools (calculators, checklists, quizzes) → use local logic only, no API calls

## Output Format

When building a tool, deliver:
1. Complete working React component
2. Integration notes for the existing app structure
3. Brief description for the blog post that will embed it
