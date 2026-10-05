# industrial-brutalist-cursor-rules

A Cursor rule for industrial / brutalist / neo-brutalist frontend design: visible grids, thick borders, hard offset shadows, flat high-saturation color blocking, and abrupt mechanical motion. Drop the `.cursor/` directory into any project and the rule becomes available to Cursor's agent.

## What's here

```
.cursor/rules/
  industrial-brutalist-ui.mdc
```

## What the rule covers

- **Identity:** loud, deliberate, built. One loud device per page (a marquee, a sticker collage, an oversized index); everything else is grid.
- **Structure:** a visible grid, 4px borders, zero-blur offset shadows, slight rotation for cards and badges only, blunt bolted-down navigation.
- **Motion:** GSAP + Lenis only, with named values (`press`, `slam-in`, `ticker`), short abrupt timing, and a `gsap.matchMedia()` reduced-motion variant.
- **Type and color:** oversized grotesk or mono display, plain body text, 2–3 flat saturated hues plus ink. No gradients, texture overlays, or glass.
- **Performance and accessibility floor:** transform/opacity only, zero layout shift, 4.5:1 contrast checked inside every color block, focus as the loudest state, full keyboard paths.

It is written as the opposite pole of [premium-luxury-cursor-rules](https://github.com/Sciontut/premium-luxury-cursor-rules). The two are meant to be used separately, never blended.

## Activation

The rule uses `alwaysApply: false` with a `description`, so Cursor's agent loads it when your prompt signals **brutalist / industrial / raw / neo-brutalist frontend** work, and stays out of unrelated tasks. To force it always-on, set `alwaysApply: true`; to scope by file type, add a `globs:` list.

## Source and history

**Current version (the commit replacing the earlier converted rule and later):** original in-house work by Michael McCollough, written as the brutalist counterpart to premium-luxury-cursor-rules. It is not derived from the earlier version described below.

**Earlier version (commits `b32cb9d` and `e533441`, June 2026):** a different rule in a "Swiss industrial print / tactical telemetry" style, condensed and adapted for Cursor from the `brutalist-skill` in [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill/tree/main/skills/brutalist-skill). Those commits credited hamzafarooq/claude-code-starter, which redistributes the same skill; the original source is Leonxlnx/taste-skill. That skill is MIT-licensed, and its copyright and permission notice, which applies to the material in those earlier commits, is reproduced in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). For that style, use the upstream skill directly.
