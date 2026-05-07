# xiaolab-component-patterns

This note collects reusable layout guidance for decks built with the published `xiaolab` skill.

## Default Template vs. Components

Use `template/index.html` as the default directly usable deck seed.

Typical default contents:
- cover,
- one main content page,
- next step page when needed.

Use `template/components/index.html` only as an optional layout reference when the default seed is not enough.

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

When the default seed feels too narrow, prefer adding:
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
