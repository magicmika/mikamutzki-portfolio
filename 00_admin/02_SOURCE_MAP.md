# 02_SOURCE_MAP

Version: 1.2
Status: current clean-source file
Project: MIKAMUTZKI — FINAL PORTFOLIO

---

## Purpose

This file tracks which sources are allowed in the clean portfolio
project and what each source is allowed to decide.

It is a source register, not a content document.

The goal is to prevent old files, old chats, screenshots, exports,
or assumptions from becoming project truth by accident.

---

## Source categories

| Category | Meaning |
|---|---|
| Truth | Current project direction, design direction, source hierarchy, or approved decisions |
| Evidence | Verified material used to support claims, cases, credentials, or project facts |
| Method | Workflow, prompting, QA, or review method; not project truth by itself |
| Archive | Historical or outdated material; may provide context but decides nothing |

---

## Status values

| Status | Meaning |
|---|---|
| `current` | Active source for the clean project |
| `pending` | Planned source, not created or not approved yet |
| `draft` | Created but not approved as current |
| `needs review` | Exists but must be checked before use |
| `historical – not in use` | Old or unsafe source; context only |
| `rejected` | Must not be used |

---

## Source register

| Source | Status | Category | Role | Allowed to decide | Not allowed to decide | Notes |
|---|---|---|---|---|---|---|
| 01_PROJECT_CHARTER.md | current | Truth | Project direction | Project purpose, Phase 1 scope, target audience, out-of-scope, speed/craft balance, decision rule | Design tokens, detailed QA rules, case details, tool workflow | Confirmed clean-source file |
| 02_SOURCE_MAP.md | current | Truth | Source hygiene | Which sources are current, pending, evidence, method, archive, or rejected | Portfolio content, design decisions, case claims | This file |
| 03_CURRENT_BASELINE.md | current | Truth | Current baseline | Confirmed starting point, open decisions, and clean-project baseline | Design tokens, content, case details, build workflow | Confirmed clean-source file |
| 04_PHASE1_DOD.md | current | Truth | Phase 1 done criteria | What "sendable" means for Phase 1, required pages, launch blockers, post-launch distinction | Design tokens, content inventory, case narrative, tool workflow | Confirmed clean-source file |
| 05_QA_METHOD.md | draft | Method | Phase 1 launch-gate QA method | QA checks for sendability, claim risk, content completeness, critical design integrity, responsive review, post-launch list | Design tokens, content, case details, legal correctness, full design-system audit | Created as draft clean-source file |
| 06_CONTENT_INVENTORY.md | draft | Evidence | Content and asset register | Known, missing, potential, and Phase-1-usable content/assets | Design tokens, QA criteria, case narratives, design decisions | Created as draft clean-source file |
| 07_CASE_FLOOM.md | draft | Evidence | Floom case source | Confirmed facts, role wording, research/testing evidence, prototype evidence, AI-claim wording, unsafe claims to avoid | Final case-page copy, final screen/process-evidence selection, design decisions | Created as draft evidence source; pending Mika approval to become current |
| 08_CASE_CUPRA.md | draft | Evidence | CUPRA case source | Document-backed/audit-backed CUPRA facts, evidence levels, role boundaries, AI-claim wording, unsafe claims to avoid, asset and permission risks | Final case-page copy, final visual selection, design decisions, public-use permission decisions | Created as draft evidence source; pending Mika approval to become current |
| 09_GALLERY_INVENTORY.md | draft | Evidence | Gallery inventory placeholder | Potential candidates, current review status, asset-label framework, rights and permission risks, open Gallery tasks | Final Gallery concept, selected assets, public-use clearance, project narratives | Created as draft placeholder; pending asset review and Mika approval |
| 10_AI_WORKFLOW_METHOD.md | draft | Method | AI workflow and prompting method | Draft rules for source governance, prompting, research, AI-assisted production, implementation support, QA and documentation | Project truth, design-system decisions, final tool stack, case claims, legal content, final publication decisions | Created as draft method source; pending Mika approval |
| Existing Figma file `wr7dHBcQcp32CGRDc9deVp` | historical – not in use | Archive | Previous design and component context | May be inspected only for a specific asset or decision after Mika explicitly requests the review | Current design authority, design tokens, component status, page structure, production sequence, implementation truth | Not a basis for the clean restart; no automatic reuse or inheritance |
| Old chats, old screenshots, old uploads, old exports, old prompts | historical – not in use | Archive | Historical context only | Nothing | Project direction, design truth, case facts, claims, QA rules, current decisions | Do not use unless Mika explicitly reclassifies a specific item |

---

## Source use rules

1. Only `current` sources can be used as active project truth.
2. `pending` sources are placeholders. They cannot decide anything yet.
3. `draft` sources need Mika approval before becoming current.
4. `needs review` sources must be checked before use.
5. `historical – not in use` sources are not allowed to decide anything.
6. If two current sources conflict, stop and flag the conflict.
7. If a needed source does not exist yet, ask Mika or mark the item as missing.
8. Do not reconstruct missing facts from memory, old chats, or assumptions.
9. Access to the existing Figma file does not make it current. Any reuse requires a concrete need, direct review, and Mika's explicit approval.

---

## Change log

| Date | Change |
|---|---|
| 2026-07-09 | v1.0 — Created clean source map |
| 2026-07-09 | v1.1 — Status updated for 03, 04 (current), 05, 06 (draft); roles and boundaries filled in; "legal advice" corrected to "legal correctness" |
| 2026-07-10 | v1.2 — Existing Figma file classified as `historical – not in use`; clean restart and explicit-review rule added |
