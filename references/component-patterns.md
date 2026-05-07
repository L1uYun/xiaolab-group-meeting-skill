# xiaolab-component-patterns

This note collects reusable layout guidance that supports the published `xiaolab` skill without bloating the main `SKILL.md`.

## Core vs. Components

Use `core/` for the smallest directly usable default deck.

Typical `core` contents:
- cover,
- one main content page,
- next step page when needed.

Use `components/` for optional layout patterns that can be assembled into real decks.

## Recommended Component Families

Preferred reusable patterns:
- text-image two-column,
- image-image comparison,
- three-column band,
- four-slot media grid,
- top-bottom split,
- left-heavy / right-light,
- right-heavy / left-light,
- process band,
- comparison zone,
- evidence band,
- metric band,
- decision board,
- collage cluster.

## What to Add First

When the library feels too narrow, prefer adding:
- stronger layout-ratio variation,
- lighter and cleaner framing,
- more flexible text-image balance,
- small combinable atoms such as dividers, pills, labels, and slots.

## What Not to Add First

Avoid growing the library mainly through narrow semantic page names such as:
- workload page,
- current judgment page,
- highlight summary page,
- before/after page.

If the same information action appears repeatedly, make it a component pattern rather than another named page.

## Cleanliness Checks

If a component page still feels noisy, inspect for:
- leftover default bullet scaffolds,
- leftover box groups,
- heavy color blocks,
- dotted image placeholders that dominate the reading,
- extra navigation dots,
- repeated skeletons with only renamed headings.

## Review Questions

Use these questions when refining components:
- Does this component support a distinct reading action?
- Is the variation structural, or only a minor width change?
- Is whitespace helping reading rhythm, or hiding weak content?
- Does the page still feel like a real meeting slide?
