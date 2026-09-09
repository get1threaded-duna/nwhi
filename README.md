# nwhi

A design engine for running design projects at scale — a library of **DESIGN.md**
files, each a complete, machine-readable design system that AI coding agents can
read to build UIs on-brand, every time.

Every design system here follows [Google's DESIGN.md format](https://github.com/google-labs-code/design.md):
a single Markdown file that pairs a YAML front matter block of design tokens
(colors, typography, spacing, radii, components) with a human-readable body that
explains the rationale. Point a coding agent at one of these files and it gets a
persistent, structured understanding of the brand — exact values *and* the
reasoning behind them.

## What's inside

```
design-md/
  superhuman/
    DESIGN.md      # Superhuman-inspired editorial/SaaS system
```

| System | Summary |
|---|---|
| [`superhuman`](design-md/superhuman/DESIGN.md) | Three-canvas editorial system — indigo-navy hero, white body, deep-teal closing band. Super Sans VF at sub-default weights (460/540/600), tight display leading, rounded-rectangle CTAs. |

More design systems drop into `design-md/<name>/DESIGN.md` over time.

## The DESIGN.md format

Each file has two layers:

1. **YAML front matter** — machine-readable tokens. Colors as CSS values,
   typography as named scales, spacing and radii as dimensions, and components
   that reference other tokens with `{path.to.token}` syntax.
2. **Markdown body** — the design rationale: overview, color usage, type
   hierarchy, layout, component specs, do's and don'ts, responsive behavior.

```yaml
---
name: Superhumon-Inspired-design-analysis
colors:
  primary: "#1b1938"
  canvas: "#ffffff"
  surface-teal-deep: "#0e3030"
typography:
  display-xxl:
    fontFamily: "'Super Sans VF', system-ui, sans-serif"
    fontSize: 64px
    fontWeight: 540
    lineHeight: 0.96
components:
  button-primary-dark:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
---

## Overview
[design philosophy and context]
```

Token references like `"{colors.primary}"` link component props back to canonical
values, so a single change propagates everywhere and stays consistent.

## Using these with the `design.md` CLI

The [`@google/design.md`](https://www.npmjs.com/package/@google/design.md) tool
validates, diffs, and exports these files. No install needed — run it with `npx`:

```bash
# Validate token references, WCAG contrast, and required sections
npx @google/design.md lint design-md/superhuman/DESIGN.md

# Compare two versions and catch regressions
npx @google/design.md diff design-md/superhuman/DESIGN.md path/to/DESIGN-v2.md

# Export tokens to a framework
npx @google/design.md export --format css-tailwind design-md/superhuman/DESIGN.md > theme.css      # Tailwind v4 @theme block
npx @google/design.md export --format json-tailwind design-md/superhuman/DESIGN.md > tailwind.theme.json  # Tailwind v3 theme.extend
npx @google/design.md export --format dtcg design-md/superhuman/DESIGN.md > tokens.json            # W3C DTCG tokens

# Print the format spec (useful to paste into an agent prompt)
npx @google/design.md spec --rules
```

`lint` exits `1` on errors and `0` when clean, so it drops straight into CI.

> On Windows PowerShell, use the alias to avoid file-association conflicts:
> `npx -p @google/design.md designmd lint design-md/superhuman/DESIGN.md`

## Using these with a coding agent

1. Give the agent the DESIGN.md for the system you're building in.
2. Ask it to build **one component at a time**, referencing token and component
   names directly (e.g. "build the pricing card using `card-pricing`").
3. Run `lint` after edits to catch broken references and contrast failures
   before rendering.
4. Follow each system's own do's/don'ts — they encode what keeps the brand
   coherent (for Superhuman: the three-canvas rhythm and the non-negotiable
   closing teal band).

## Adding a design system

1. Create `design-md/<name>/DESIGN.md`.
2. Fill the front matter with `colors`, `typography`, `spacing`, `rounded`, and
   `components` tokens; write the body sections.
3. Run `npx @google/design.md lint design-md/<name>/DESIGN.md` until it's clean.
4. Add a row to the table above.

## Credits

- Format & tooling: [google-labs-code/design.md](https://github.com/google-labs-code/design.md)
- Design systems are inspired interpretations for analysis and prototyping, not
  official brand assets.
