---
version: alpha
name: Caveman-Primal-design-analysis
description: A self-authored primal/paleo design language — a "carved from stone and lit by fire" system built on a three-canvas rhythm of burnt-charcoal soot for the monumental hero, warm parchment limestone for the body, and a fire-ember closing band. Headlines are monumental condensed caps (chiseled, lightly letter-spaced, near-black slab weight); body is a sturdy earthy slab. The palette is drawn from cave-painting pigments — soot black, red-ochre ember, yellow-earth ochre, terracotta clay, bone and limestone. Edges are hard and chipped (near-zero radii), buttons are square-cut, and depth comes from carved insets and firelight rather than soft shadows. It reads more like a hand-hewn stone monument than a modern SaaS app.

colors:
  primary: "#241d17"
  primary-deep: "#150f0b"
  ember: "#a83a16"
  ember-deep: "#7f2b0f"
  ochre: "#c98a34"
  clay: "#9a5738"
  moss: "#6f6f3d"
  bone: "#efe7d6"
  canvas: "#e7ddc8"
  canvas-soft: "#ded2b9"
  stone: "#8a7d68"
  hairline: "#cbbc98"
  hairline-dark: "#4a3f2e"
  ink: "#2b2318"
  ink-mute: "#63563f"
  ink-faint: "#8a7d68"
  on-primary: "#efe7d6"
  on-dark-mute: "#b8ac97"
  on-dark-faint: "#7d7057"

typography:
  display-xxl:
    fontFamily: "'Monolith', 'Oswald', 'Arial Narrow', system-ui, sans-serif"
    fontSize: 72px
    fontWeight: 700
    lineHeight: 0.92
    letterSpacing: 0.5px
  display-xl:
    fontFamily: "'Monolith', 'Oswald', 'Arial Narrow', system-ui, sans-serif"
    fontSize: 52px
    fontWeight: 700
    lineHeight: 0.94
    letterSpacing: 0.5px
  display-lg:
    fontFamily: "'Monolith', 'Oswald', 'Arial Narrow', system-ui, sans-serif"
    fontSize: 34px
    fontWeight: 700
    lineHeight: 1.0
    letterSpacing: 0.4px
  display-md:
    fontFamily: "'Monolith', 'Oswald', 'Arial Narrow', system-ui, sans-serif"
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: 0.3px
  heading-lg:
    fontFamily: "'Monolith', 'Oswald', 'Arial Narrow', system-ui, sans-serif"
    fontSize: 20px
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: 0.3px
  body-lg:
    fontFamily: "'Flint', 'Zilla Slab', Georgia, 'Times New Roman', serif"
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: 0
  body-md:
    fontFamily: "'Flint', 'Zilla Slab', Georgia, 'Times New Roman', serif"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: 0
  body-strong:
    fontFamily: "'Flint', 'Zilla Slab', Georgia, 'Times New Roman', serif"
    fontSize: 17px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: 0
  button-md:
    fontFamily: "'Monolith', 'Oswald', 'Arial Narrow', system-ui, sans-serif"
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.0
    letterSpacing: 1px
  button-cap:
    fontFamily: "'Monolith', 'Oswald', 'Arial Narrow', system-ui, sans-serif"
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1.0
    letterSpacing: 1.2px
  caption:
    fontFamily: "'Flint', 'Zilla Slab', Georgia, 'Times New Roman', serif"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0
  micro:
    fontFamily: "'Flint', 'Zilla Slab', Georgia, 'Times New Roman', serif"
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0.2px

rounded:
  xs: 0px
  sm: 1px
  md: 2px
  lg: 4px
  xl: 8px
  full: 9999px

spacing:
  xxs: 2px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  xxl: 40px
  huge: 72px

components:
  button-ember:
    backgroundColor: "{colors.ember}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button-md}"
    rounded: "{rounded.md}"
    padding: 14px 24px
  button-ember-pressed:
    backgroundColor: "{colors.ember-deep}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button-md}"
    rounded: "{rounded.md}"
    padding: 14px 24px
  button-on-dark:
    backgroundColor: "{colors.bone}"
    textColor: "{colors.primary}"
    typography: "{typography.button-md}"
    rounded: "{rounded.md}"
    padding: 14px 24px
  button-outline:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.button-md}"
    rounded: "{rounded.md}"
    padding: 14px 24px
  button-on-ember:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button-md}"
    rounded: "{rounded.md}"
    padding: 14px 24px
  text-input:
    backgroundColor: "{colors.canvas-soft}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 12px 14px
  card-feature-light:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 40px
  card-pricing:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 40px
  card-pricing-featured:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: 40px
  card-ember-band:
    backgroundColor: "{colors.ember}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-lg}"
    rounded: "{rounded.lg}"
    padding: 72px
  card-feature-row:
    backgroundColor: "{colors.canvas-soft}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 24px
  tab-chisel:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.button-cap}"
    rounded: "{rounded.sm}"
    padding: 10px 18px
  nav-bar-dark:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xs}"
    padding: 16px 24px
  nav-bar-light:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xs}"
    padding: 16px 24px
  link-on-light:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xs}"
    padding: 0px
  footer-dark:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-dark-mute}"
    typography: "{typography.caption}"
    rounded: "{rounded.xs}"
    padding: 72px 24px
---

## Overview

Caveman is a made-from-scratch primal design language: **carved from stone, lit by fire.** It runs on a three-canvas rhythm that echoes the way the superhuman system splits dark hero / light body / accent close — but reinterpreted in earth pigment.

The hero opens in **burnt charcoal** `{colors.primary}` (`#241d17` — a warm soot near-black, never pure `#000`), overlaid with a subtle firelight vignette and, where possible, a hand-drawn cave-painting motif (ochre animal or handprint) bleeding off one edge. Headlines render in `{typography.display-xxl}` — monumental condensed **caps** at slab weight 700 with a slight positive `0.5px` letter-spacing, so the type reads as chiseled into rock rather than typed. A single square-cut `button-ember` anchors each band — the CTA is always the fire.

The body flips to **parchment limestone**. `{colors.canvas}` (`#e7ddc8`) takes over below the hero, with body copy in `{colors.ink}` (`#2b2318` — a warm umber, never black) set in the sturdy earthy slab `{typography.body-md}`. Feature rows alternate between parchment and the deeper sand `{colors.canvas-soft}`. Pricing sits on this surface; the featured tier inverts to charcoal, completing the light/dark polarity.

Every page closes with a **fire-ember band** (`{colors.ember}` — `#a83a16` — red-ochre, the cave-painting pigment). The ember is the single chromatic release of the page: the closing headline in `{typography.display-lg}` over ember, resolved by a dark square-cut `button-on-ember`. Charcoal → parchment → ember is the whole system; a fourth canvas breaks it.

**Key Characteristics:**
- Three-canvas system: soot charcoal (`{colors.primary}`) for the hero, parchment (`{colors.canvas}`) for the body, fire-ember (`{colors.ember}`) for the closing band.
- Monumental condensed **caps** headlines — chiseled slab weight 700 with a light positive `0.5–1px` letter-spacing, the "carved in stone" signature.
- Hard, chipped edges — near-zero radii (`{rounded.md}` is 2px); the CTA is a square-cut block, never a pill.
- Cave-pigment palette only — soot, red-ochre ember, yellow-earth ochre, terracotta clay, bone, limestone. No blues, no neon.
- Warm umber body ink (`#2b2318`) — never pure black; the whole system is warm-biased.
- Fire is the CTA — the ember accent belongs to actions and the closing band, nowhere decorative.
- Sturdy slab body (`{typography.body-md}`) against monumental condensed display — the two-voice contrast of monument and hand.

## Colors

> **Source:** Self-authored primal/paleo concept system (no external brand). Pigments are drawn from the cave-painting canon: charcoal soot, red- and yellow-ochre, terracotta, and bone/limestone grounds.

### Brand & Accent
- **Soot Charcoal** (`{colors.primary}` — `#241d17`): Primary dark surface. Hero canvas, featured pricing tier, dark nav, footer, and the button on the ember band. Warm near-black, never `#000`.
- **Charcoal Deep** (`{colors.primary-deep}` — `#150f0b`): Deepest soot — hero gradient floor and pressed-dark states.
- **Fire Ember** (`{colors.ember}` — `#a83a16`): The signature accent — red-ochre pigment. Owns the primary CTA and the closing band. Fire = action.
- **Ember Deep** (`{colors.ember-deep}` — `#7f2b0f`): Pressed state for the ember CTA.
- **Yellow Ochre** (`{colors.ochre}` — `#c98a34`): Secondary earth accent — rules, small marks, and accent text **on charcoal only** (5.3:1 on soot). Used sparingly.
- **Terracotta Clay** (`{colors.clay}` — `#9a5738`): Tertiary warm accent for decorative fills and category marks.
- **Dry Moss** (`{colors.moss}` — `#6f6f3d`): Rare olive-earth accent — the one cool-leaning pigment, used for the occasional tag or illustration stroke.

### Surface
- **Parchment Canvas** (`{colors.canvas}` — `#e7ddc8`): Default body background — cave-wall limestone.
- **Sand Soft** (`{colors.canvas-soft}` — `#ded2b9`): Deeper sand for alternating feature-row bands and input fills.
- **Bone** (`{colors.bone}` — `#efe7d6`): Lightest ground — light text on dark, and the `button-on-dark` fill over the hero.
- **Stone** (`{colors.stone}` — `#8a7d68`): Mid grey-brown for dividers and muted chrome.
- **Hairline** (`{colors.hairline}` — `#cbbc98`): 1px warm-sand borders on light surfaces.
- **Hairline Dark** (`{colors.hairline-dark}` — `#4a3f2e`): 1px borders on charcoal surfaces.

### Text
- **Ink** (`{colors.ink}` — `#2b2318`): Default body text — warm umber, never pure black (11.8:1 on parchment).
- **Ink Mute** (`{colors.ink-mute}` — `#63563f`): Secondary text and captions on light (5.3:1 on parchment).
- **Ink Faint** (`{colors.ink-faint}` — `#8a7d68`): Tertiary / disabled text and decorative labels.
- **On Primary** (`{colors.on-primary}` — `#efe7d6`): Bone text on charcoal and ember (13.5:1 on soot, 5.2:1 on ember).
- **On Dark Mute** (`{colors.on-dark-mute}` — `#b8ac97`): Secondary text on dark (footer, sub-labels).
- **On Dark Faint** (`{colors.on-dark-faint}` — `#7d7057`): Tertiary/decorative text on dark — never body copy.

## Typography

### Font Family

The display and UI tier is **Monolith** — a proprietary monumental condensed display face, used in **caps** at slab weight 700 with slight positive tracking so headlines read as carved into rock.

The reading tier is **Flint** — a sturdy earthy slab serif with weights 400 / 500 / 700, warm and grounded against the monumental caps.

For substitution, use **Oswald** (open-source variable condensed sans, Google Fonts) for the Monolith tier — set weight 600–700 and `text-transform: uppercase`. Use **Zilla Slab** (open-source slab serif, Google Fonts) for the Flint tier at 400 / 500 / 700. The condensed-caps-over-slab pairing is the system's two-voice signature: monument and hand.

### Hierarchy

| Token | Size | Weight | Line Height | Letter Spacing | Use |
|---|---|---|---|---|---|
| `{typography.display-xxl}` | 72px | 700 | 0.92 | 0.5px | Hero headline (CAPS) |
| `{typography.display-xl}` | 52px | 700 | 0.94 | 0.5px | Section opener (CAPS) |
| `{typography.display-lg}` | 34px | 700 | 1.0 | 0.4px | Closing-band / feature title (CAPS) |
| `{typography.display-md}` | 24px | 700 | 1.05 | 0.3px | Card title (CAPS) |
| `{typography.heading-lg}` | 20px | 600 | 1.1 | 0.3px | Compact card title (CAPS) |
| `{typography.body-lg}` | 19px | 400 | 1.55 | 0 | Marketing body lead |
| `{typography.body-md}` | 16px | 400 | 1.55 | 0 | Default UI body |
| `{typography.body-strong}` | 17px | 700 | 1.5 | 0 | Emphasized body |
| `{typography.button-md}` | 16px | 700 | 1.0 | 1px | Square-cut button label (CAPS) |
| `{typography.button-cap}` | 13px | 700 | 1.0 | 1.2px | Compact button / tab label (CAPS) |
| `{typography.caption}` | 14px | 400 | 1.4 | 0 | Helper, footnote |
| `{typography.micro}` | 12px | 500 | 1.4 | 0.2px | Fine print, tag label |

### Principles
- **Monumental caps.** Every display and button tier is set in caps at slab weight 700 — the type is meant to look chiseled, not typed.
- **Positive tracking on display.** `0.3–1px` of letter-spacing opens the condensed caps into a carved, monumental rhythm (the inverse of the tight negative tracking a modern SaaS sans would use).
- **Two voices.** Condensed caps display + sturdy slab body. Never set body copy in the display face, and never set headlines in the slab.
- **Tight display leading.** `0.92` on 72px — the monumental caps stack into a dense stone-tablet block.

### Note on Font Substitutes
**Oswald** (display, `wght` 600–700, uppercase) and **Zilla Slab** (body, 400/500/700) are the recommended open-source substitutes, both on Google Fonts. Apply `text-transform: uppercase` and `letter-spacing: 0.5px` to the Oswald tier to reproduce the carved-caps signature; do not letter-space the Zilla Slab body.

## Layout

### Spacing System
- **Base unit**: 8px (with 2 / 4 / 12 sub-tokens for fine work).
- **Tokens**: `{spacing.xxs}` 2px · `{spacing.xs}` 4px · `{spacing.sm}` 8px · `{spacing.md}` 12px · `{spacing.lg}` 16px · `{spacing.xl}` 24px · `{spacing.xxl}` 40px · `{spacing.huge}` 72px.
- **Section padding**: 72–112px on most sections; the closing ember band uses 96–128px for monumental weight.
- **Card internal padding**: 40px on feature and pricing cards; 24px on alternating feature rows.

### Grid & Container
- Hero spans the full viewport with the firelight vignette edge-to-edge; content centers in a ~1000px column.
- Body content centers in ~1000–1120px.
- Pricing collapses 3-up → 2-up → 1-up at 1024 / 768 breakpoints.

### Whitespace Philosophy
Caveman uses heavy, deliberate whitespace — the monument needs air. Section gaps run toward 96px; the ember closing band gets up to 128px of vertical weight. The blank parchment is part of the "ancient and unhurried" feel.

## Elevation & Depth

| Level | Treatment | Use |
|---|---|---|
| 0 | Flat | Default surface |
| 1 | `box-shadow: inset 0 -2px 0 rgba(21,15,11,0.25)` | Carved inset — the chipped-stone lift |
| 2 | `box-shadow: 0 6px 20px rgba(21,15,11,0.28)` | Floating panels, modals |
| 3 | Firelight vignette (radial ember-to-soot over charcoal) | The hero's depth medium |

### Decorative Depth
The hero's depth is the **firelight vignette** — a soft radial wash from warm ember at the lower edge up into `{colors.primary-deep}`, as if a fire lights the bottom of the cave wall. Implemented as a CSS radial gradient. Cards on parchment favor a **carved inset** (a 2px dark bottom-edge shadow) over soft drop shadows — surfaces look chipped into stone, not floated above it.

## Shapes

### Border Radius Scale

| Token | Value | Use |
|---|---|---|
| `{rounded.xs}` | 0px | Nav bars, links, footer — raw square edges |
| `{rounded.sm}` | 1px | Form inputs, tabs |
| `{rounded.md}` | 2px | Buttons — the signature square-cut block |
| `{rounded.lg}` | 4px | Cards, pricing, closing band |
| `{rounded.xl}` | 8px | Large modals |
| `{rounded.full}` | 9999px | Reserved for round pictographic marks (handprint, sun) only — never buttons |

### Geometry & Marks
The recurring visual is the **cave-painting mark** — hand-drawn ochre pictographs (handprints, animals, tally strokes) rendered as flat single-color SVG in `{colors.ochre}` or `{colors.clay}` over charcoal. Edges everywhere else stay hard and near-square; the roughness lives in the pigment marks and textures, not in rounded corners.

## Components

### Buttons

**`button-ember`** — the dominant square-cut CTA. Fire is action.
- Background `{colors.ember}`, text `{colors.on-primary}`, type `{typography.button-md}` (caps), padding `14px 24px`, rounded `{rounded.md}` 2px.
- Pressed state `button-ember-pressed` shifts to `{colors.ember-deep}`.

**`button-on-dark`** — the CTA over the charcoal hero, in bone.
- Background `{colors.bone}`, text `{colors.primary}`, same type/shape/padding. Used where ember would vibrate against a busy hero vignette.

**`button-outline`** — the quiet secondary on parchment.
- Background `{colors.canvas}`, text `{colors.ink}`, 1px solid `{colors.hairline-dark}` border, same square-cut shape.

**`button-on-ember`** — the CTA inside the closing ember band.
- Background `{colors.primary}` (charcoal), text `{colors.on-primary}`, square-cut. A dark block resolving the fire band.

### Cards & Containers

**`card-feature-light`** — feature card on parchment.
- Background `{colors.canvas}`, padding `{spacing.xxl}` 40px, rounded `{rounded.lg}` 4px, 1px `{colors.hairline}` border, carved-inset bottom edge.

**`card-pricing`** — standard pricing tier.
- Background `{colors.canvas}`, padding 40px, rounded `{rounded.lg}`, 1px `{colors.hairline}` border.

**`card-pricing-featured`** — inverted charcoal featured tier.
- Background `{colors.primary}`, text `{colors.on-primary}`, otherwise identical to `card-pricing`.

**`card-ember-band`** — the closing CTA band on every page.
- Background `{colors.ember}`, text `{colors.on-primary}`, padding `{spacing.huge}` 72px, rounded `{rounded.lg}` (usually full-bleed and radius-less in practice). Holds a `{typography.display-lg}` closing headline in caps and a single `button-on-ember`.

**`card-feature-row`** — alternating feature-row card on the body.
- Background `{colors.canvas-soft}`, text `{colors.ink}`, padding `{spacing.xl}` 24px, rounded `{rounded.md}` 2px. Used in pairs/triplets below the hero.

### Inputs & Forms

**`text-input`** — standard form input.
- Background `{colors.canvas-soft}`, text `{colors.ink}`, type `{typography.body-md}`, padding `12px 14px`, rounded `{rounded.sm}` 1px, 1px `{colors.hairline}` border. Inputs read as recessed into the stone.

### Navigation

**`nav-bar-dark`** — top nav over the charcoal hero.
- Background `{colors.primary}`, text `{colors.on-primary}`, padding `{spacing.lg} {spacing.xl}`, rounded `{rounded.xs}` 0px. Logo left, nav center, a `button-on-dark` at the right.

**`nav-bar-light`** — top nav on body / pricing pages.
- Background `{colors.canvas}`, text `{colors.ink}`, same structure with a `button-ember` at the right.

### Tabs, Tags, and Chips

**`tab-chisel`** — feature-category tab selector.
- Background `{colors.canvas}`, text `{colors.ink}`, type `{typography.button-cap}` (caps), padding `10px 18px`, rounded `{rounded.sm}` 1px. Square-cut, never a pill; the active tab fills `{colors.primary}` with bone text.

### Signature Components

**Firelit Hero** — a charcoal band with the firelight vignette rising from the lower edge, a cave-painting ochre mark bleeding off one side, a monumental caps headline in `{typography.display-xxl}`, and a single `button-ember`. The brand's opening chord.

**Closing Ember Band** — every page closes with a `card-ember-band`: a `{typography.display-lg}` caps headline over fire-ember, resolved by a dark `button-on-ember`. The page's final, warm release.

**`link-on-light`** — inline links on the body.
- Text `{colors.ink}` in `{typography.body-md}` with a persistent 2px `{colors.ember}` underline — the link is marked in ochre.

**`footer-dark`** — site-wide footer.
- Background `{colors.primary}`, text `{colors.on-dark-mute}`, type `{typography.caption}`, padding `{spacing.huge} {spacing.xl}` (72px 24px), rounded `{rounded.xs}` 0px. Four columns of link groups over charcoal, with an ochre pictographic mark and a small legal row.

## Do's and Don'ts

### Do
- Keep the three-canvas rhythm: charcoal hero → parchment body → ember closing band.
- Set every display and button tier in **caps** with positive `0.3–1px` tracking — the carved-in-stone signature.
- Reserve ember for actions and the closing band; fire means "do this."
- Use warm umber `{colors.ink}` for body text — never pure black.
- Keep edges hard: 2px on buttons, 4px on cards, 0px on nav/footer.
- Let cave-painting ochre marks (handprints, animals, tallies) carry the decorative roughness.

### Don't
- Don't round buttons into pills — the square-cut block is the brand; `{rounded.full}` is for round pictographs only.
- Don't set body copy in the condensed display face, or headlines in the slab — keep the two voices apart.
- Don't introduce cool colors (blue, teal, neon) — the palette is soot, ember, ochre, clay, and bone only.
- Don't render body text in pure black — the warm umber `#2b2318` is the brand.
- Don't omit the closing ember band — every marketing page resolves in fire.
- Don't lean on soft drop shadows for card lift; prefer the carved 2px inset.

## Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|---|---|---|
| Wide | ≥ 1440px | Full firelight vignette; ember band 128px tall; hero display at 72px |
| Desktop | 1024–1440px | Default content max-width; pricing 3-up |
| Tablet | 768–1023px | Pricing 2-up; cave-painting mark crops in |
| Mobile | < 768px | Pricing 1-up; hamburger nav; hero display drops 72 → 40px |

### Touch Targets
- Buttons hit ≥ 44×44px on mobile via 14px vertical padding × 16px line-height. WCAG AAA.
- Form fields stay at the 44px minimum height.

### Collapsing Strategy
- Display tiers stair-step 72 → 52 → 40 → 30 → 24px.
- The firelight vignette simplifies to a flat charcoal on mobile; the ochre mark crops to a corner.
- Pricing tiers stair-step 3-up → 2-up → 1-up.
- Top nav collapses to a hamburger below 768px.
- Closing ember band reduces vertical padding from 128 → 72px on mobile.

### Image Behavior
Cave-painting marks are flat single-color SVG and scale cleanly at any size. The hero vignette uses a CSS radial gradient (no raster), so it never needs `srcset`; any photographic texture uses desktop / mobile crops.

## Iteration Guide

1. Focus on ONE component at a time.
2. Reference component names and tokens directly (e.g. "build the pricing card using `card-pricing`").
3. Run `npx @google/design.md lint DESIGN.md` after edits.
4. Default body to `{typography.body-md}`; reserve `{typography.body-lg}` for marketing leads.
5. Keep the three-canvas rhythm (charcoal / parchment / ember) — adding a fourth canvas color breaks the system.
6. The closing ember band is non-negotiable — every marketing page resolves in fire.
