# 05_QA_METHOD

Version: 1.1
Status: draft clean-source file
Project: MIKAMUTZKI — FINAL PORTFOLIO

---

## Purpose

This file defines the QA method for Phase 1 of the portfolio.

It is a launch gate, not a complete design-system audit.

The single question it answers is:

> Is the portfolio sendable — yes or no?

This file does not contain design tokens, content, or case details.
It only defines what must be checked before Phase 1 can be treated
as ready to send.

---

## QA scope

This QA covers Phase 1 only:
Home, Work / Gallery, Floom case, CUPRA case, Contact,
Impressum, Datenschutz.

Later phases may require a separate or extended QA method.

---

## Review categories

### 1. Sendability

The minimum bar. If any item here fails, the portfolio is not sendable.

| Check | Pass criteria |
|---|---|
| All Phase 1 pages exist and load | No missing pages, no broken routes |
| Navigation works on desktop and mobile | All links reach the correct destination |
| Contact page is functional | Email address or form works |
| Impressum is present and not placeholder | Current legal text is inserted, readable, and reachable |
| Datenschutz is present and not placeholder | Current legal text is inserted, readable, and reachable |
| No placeholder text visible | No TBD, Lorem ipsum, or empty sections |

---

### 2. Claim risk

Unverifiable or invented claims block sendability.

| Check | Pass criteria |
|---|---|
| No invented KPIs or outcomes | Every metric has a real source |
| No invented client names or project roles | Every claim matches confirmed evidence |
| No testimonials or awards without source | Either remove or confirm with source |
| No generic self-description | Avoid terms such as "passionate", "innovative", "creative thinker", "out-of-the-box"; replace with specific, evidence-based statements |

---

### 3. Content completeness

| Check | Pass criteria |
|---|---|
| All Phase 1 pages have real copy | No section is empty or draft-only |
| Floom case has copy, screens, and process evidence | All three present and confirmed |
| CUPRA case has copy and visuals | Both present and confirmed |
| Work / Gallery has curated images | At least a minimum viable selection |
| Home has headline and intro copy | Both present and confirmed |

---

### 4. Design integrity

Critical violations only. This is not a full component audit.

| Check | Pass criteria |
|---|---|
| No known critical radius violation | Radius follows the confirmed design direction; no accidental soft SaaS rounding, pill buttons, circular icon buttons, or rounded cards |
| No unapproved #FFFFFF usage | Pure white does not appear in backgrounds, text, strokes, surfaces, or UI elements unless explicitly approved |
| Only Switzer is in use | No other typeface appears anywhere on the site |
| No generic SaaS / startup-template aesthetic | Visual language is clearly Mika's own |
| No obvious AI-slop or template defaults | No shadcn, Material UI, or neobrutalist defaults visible |
| Typography is consistent across all pages | One type system, no mixups |
| Spacing and layout are consistent | No broken grids or orphaned elements |

---

### 5. Mobile and desktop

| Check | Pass criteria |
|---|---|
| All pages are usable on mobile | No broken layouts, no hidden content |
| All pages are usable on desktop | No broken layouts, no oversized gaps |
| Navigation is usable on both | No hidden or inaccessible nav items |

---

### 6. Post-launch list

Items that do not block launch but must be addressed after Phase 1 goes live.

| Item | Priority | Notes |
|---|---|---|
| TBD | — | To be added during QA review |

---

## How to use this file

1. Run this QA before treating any Phase 1 page as done.
2. Every failed check must be resolved or explicitly accepted by Mika
   before launch.
3. Post-launch items must be logged in the post-launch list,
   not silently ignored.
4. This file is a method document. It does not replace
   the Content Inventory or the Phase 1 Definition of Done.

---

## Change log

| Date | Change |
|---|---|
| 2026-07-09 | v1.0 — Created as lean Phase 1 launch-gate QA method |
| 2026-07-09 | v1.1 — Four corrections applied: legal wording, claim language, radius rule, #FFFFFF scope |
| 2026-07-10 | v1.2 — Typography rule generalised to positive-list format (Switzer only), removed reference to unrelated typefaces |

