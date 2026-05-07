---
name: xiaolab
description: Use when creating or refining Xiaolab-style HTML group-meeting decks with a minimal core deck plus a reusable components gallery.
version: 1.5.0
author: Hermes Agent
license: Apache-2.0
metadata:
  hermes:
    tags: [xiaolab, group-meeting, html-deck, ppt-template, component-library]
    related_skills: [open-design, productivity-skill-router, creative/claude-design]
---

# Xiaolab Group-Meeting Decks

## Overview

This skill is for building Xiaolab-style HTML group-meeting decks that stay light, clean, and reusable.

The core idea is simple:
- keep the default deck very small,
- move variety into reusable layout components,
- and avoid turning the template into a half-written presentation.

Use it to create a new deck, refactor an existing Xiaolab template, or review whether a generated deck still feels like a real lab meeting rather than a template demo.

## When to Use

Use this skill when you need to:
- create a Xiaolab-style HTML group-meeting deck,
- refactor a template into a smaller default deck plus reusable components,
- expand layout variety without adding many narrow semantic page types,
- clean visible template noise from a deck,
- review whether a generated deck still reads like a real weekly meeting.

Do not use this skill for:
- generic slide design unrelated to Xiaolab,
- repository maintenance or GitHub workflow,
- internal reviewer playbooks or agent-only troubleshooting notes.

## Design Principles

### 1. Organize by message first, pages second

Do not start by filling a large predefined deck.

Preferred order:
1. decide the message,
2. decide how many pages are actually needed,
3. select layouts from the component library,
4. add only what is still missing.

The template serves the presentation.
The presentation should not be bent to fit the template.

### 2. Keep the default deck minimal

A normal group-meeting deck usually needs only:
- a cover,
- one main content page,
- a next-step page when needed.

Everything else should be treated as optional components, not default required pages.

### 3. Prefer empty structure over fake content

The HTML template should not ship with visible placeholder content such as:
- sample paragraphs,
- teaching text,
- visible `{{title}}`-style placeholders,
- default metric blocks,
- default bullet scaffolds,
- decorative process arrows,
- heavy default cards or panels.

What may remain:
- minimal cover identifiers,
- empty text regions,
- empty media regions,
- layout skeletons.

### 4. Keep guidance off the visible page

Visible pages should not contain template meta-language such as:
- `核心页 / 参考页`,
- `备注：...`,
- "use this page when...",
- "if the first few pages are enough...".

The overview should also stay clean:
- keep page number and page name,
- include a real page title only when one actually exists,
- do not expose notes, summaries, or teaching text.

## Output Structure

When the template is meant to stay reusable, prefer a two-layer output structure:

1. `core/index.html`
   - the minimal default deck,
   - usually cover / main content / next step.
2. `components/index.html`
   - the reusable layout gallery,
   - a place for optional composition patterns.

This is better than forcing both roles into a single large deck.

## Recommended Directory Shape

Keep the template in this form:
- `template/core/index.html`
- `template/components/index.html`
- `template/assets/*`

Avoid keeping obsolete one-off files such as:
- old `template/index.html`,
- old split slide files like `slide4.html`, `slide5.html`, `slide6.html`,
- temporary drafting files.

## Component Strategy

The goal is not to invent more and more semantic slide names.
The goal is to maintain a reusable set of layout primitives.

Useful component families include:
- text-image two-column layouts,
- image-image comparisons,
- three-column bands,
- four-slot media grids,
- top-bottom layouts,
- left-heavy / right-light layouts,
- right-heavy / left-light layouts,
- process bands,
- comparison zones.

When expanding the library, prefer:
- stronger layout variation,
- lighter framing,
- more flexible text-image ratios,
- composable small atoms such as lines, dividers, pills, tiny labels, and slots.

Avoid expanding mainly through narrow semantic page types such as:
- workload page,
- current judgment page,
- highlight summary page,
- before/after page.

See `references/component-patterns.md` for the extended component notes.

## Cleanliness Rules

If a page still feels templated or noisy, check for these first:
- leftover default bullet structures,
- leftover box groups,
- heavy default panels or color blocks,
- dotted image placeholders that dominate the page,
- extra navigation dots,
- overview cards leaking notes or summaries,
- components that were renamed but still share almost the same skeleton.

## Realism Rules

A good Xiaolab deck should feel like an actual group meeting.
It should not feel like a template manual.

Signs of a better deck:
- each page performs one clear job,
- titles match the amount of real content,
- large whitespace is used for rhythm, not to hide weak content,
- components differ by information action, not only by column ratio,
- the deck reads like weekly progress, evidence, uncertainty, and next steps.

## Common Pitfalls

1. **Too many default pages.**
   If the deck already feels long before real content arrives, reduce the core deck first.

2. **Semantic page-type explosion.**
   If every need becomes a new named page, convert recurring patterns into components instead.

3. **Visible template language on the slide.**
   Remove instructional labels, remarks, and sample prose from the rendered page.

4. **Heavy decoration hiding weak structure.**
   Reduce panels, boxes, and ornamental framing before adding more text.

5. **Dirty overview cards.**
   Overview entries should not expose notes, summaries, or hidden author guidance.

6. **Different names, same skeleton.**
   If several components feel identical in use, increase structural variation rather than renaming them.

## Verification Checklist

- [ ] The default deck is minimal rather than exhaustive.
- [ ] Optional variety lives in `components/`, not in many default pages.
- [ ] No visible placeholder prose or teaching text remains in the rendered deck.
- [ ] Overview cards expose only clean navigation information.
- [ ] Components differ by reading action and rhythm, not just by small width changes.
- [ ] The deck feels like a real group meeting, not a template showcase.
- [ ] Directory structure matches `core/ + components/ + assets/`.
