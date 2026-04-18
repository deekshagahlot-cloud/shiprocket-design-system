# Shiprocket Design System Tokens

This repository contains the single source of truth for all design tokens used across Shiprocket's product.

## Folder Structure

```
tokens/
├── colors.json      → All raw color values (primary, neutral, semantic, accent)
├── typography.json  → Font family, size scale, line heights, weights
├── spacing.json     → Spacing scale (space-1 to space-9)
├── radius.json      → Border radius values
└── components.json  → Component-level tokens (button, badge, toaster, banner, tag)
```

## How to use with AI

Paste any token file into Claude or another AI tool and say:
> "Use these design tokens to build [component name] for Shiprocket"

The AI will use the correct colors, spacing, and radius from your system.

## Token naming convention

- Raw tokens: `color.primary.500`, `spacing.space-4`, `radius.md`
- Component tokens reference raw tokens using `{token.name}` syntax
- Example: `button.primary.bg-default → {color.primary.500} → #7458E7`

## Color rule

| Part | Token level |
|------|-------------|
| Background | 50 shade |
| Icon / Text / Border | 500 shade |
| Body text inside component | neutral.800 |
| Dismiss / close icon | neutral.600 |

## Maintained by

Shiprocket Design Team
