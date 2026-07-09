# 02_SOURCE_MAP

Version: 1.0  
Status: current clean-source file  
Project: MIKAMUTZKI — FINAL PORTFOLIO

## Purpose

This file tracks which sources are allowed in the clean portfolio project and what each source is allowed to decide.

It is a source register, not a content document.

The goal is to prevent old files, old chats, screenshots, exports, or assumptions from becoming project truth by accident.

## Source categories

| Category | Meaning |
|---|---|
| Truth | Current project direction, design direction, source hierarchy, or approved decisions |
| Evidence | Verified material used to support claims, cases, credentials, or project facts |
| Method | Workflow, prompting, QA, or review method; not project truth by itself |
| Archive | Historical or outdated material; may provide context but decides nothing |

## Status values

| Status | Meaning |
|---|---|
| current | Active source for the clean project |
| pending | Planned source, not created or not approved yet |
| draft | Created but not approved as current |
| needs review | Exists but must be checked before use |
| historical – not in use | Old or unsafe source; context only |
| rejected | Must not be used |

## Source register

| Source | Status | Category | Role | Allowed to decide | Not allowed to decide | Notes |
|---|---|---|---|---|---|---|
| 01_PROJECT_CHARTER.md | current | Truth | Project direction | Project purpose, Phase 1 scope, target audience, out-of-scope, speed/craft balance, decision rule | Design tokens, detailed QA rules, case details, tool workflow | Confirmed clean-source file |
| 02_SOURCE_MAP.md | current | Truth | Source hygiene | Which sources are current, pending, evidence, method, archive, or rejected | Portfolio content, design decisions, case claims | This file |
| 03_CURRENT_BASELINE.md | pending | Truth | Current baseline | TBD | TBD | Not created yet |
| 04_PHASE1_DOD.md | pending | Truth | Phase 1 done criteria | TBD | TBD | Not created yet |
| 05_QA_METHOD.md | pending | Method | QA and review method | TBD | TBD | Not created yet |
| 06_CONTENT_INVENTORY.md | pending | Evidence | Available content and assets | TBD | TBD | Not created yet |
| 07_CASE_FLOOM.md | pending | Evidence | Floom case source | TBD | TBD | Not created yet |
| 08_CASE_CUPRA.md | pending | Evidence | CUPRA case source | TBD | TBD | Not created yet |
| 09_GALLERY_INVENTORY.md | pending | Evidence | Gallery source | TBD | TBD | Not created yet |
| 10_AI_WORKFLOW_METHOD.md | pending | Method | AI workflow and prompting method | TBD | TBD | Not created yet |
| Old chats, old screenshots, old uploads, old exports, old prompts | historical – not in use | Archive | Historical context only | Nothing | Project direction, design truth, case facts, claims, QA rules, current decisions | Do not use unless Mika explicitly reclassifies a specific item |

## Source use rules

1. Only `current` sources can be used as active project truth.
2. `pending` sources are placeholders. They cannot decide anything yet.
3. `draft` sources need Mika approval before becoming current.
4. `needs review` sources must be checked before use.
5. `historical – not in use` sources are not allowed to decide anything.
6. If two current sources conflict, stop and flag the conflict.
7. If a needed source does not exist yet, ask Mika or mark the item as missing.
8. Do not reconstruct missing facts from memory, old chats, or assumptions.

## Change log

| Date | Change |
|---|---|
| 2026-07-09 | Created clean source map v1.0 |