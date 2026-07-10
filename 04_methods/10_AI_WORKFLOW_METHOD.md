# 10_AI_WORKFLOW_METHOD

Version: 0.1  
Status: draft method source  
Project: MIKAMUTZKI — FINAL PORTFOLIO  
Area: AI workflow / prompting / production method  
Category: Method

---

## Purpose

This file defines a draft method for using AI responsibly inside the MIKAMUTZKI — FINAL PORTFOLIO project.

It is a method source, not project truth, not a design-system specification, not a case source, and not a tool workflow finalisation.

The goal is to support speed, structure, visual exploration, copy drafting, QA, and documentation without allowing AI output to invent claims, replace evidence, flatten Mika's visual judgment, or create generic portfolio material.

This file needs Mika's approval before it can become a current method source.

---

## Scope

This method may support:

- source structuring
- evidence extraction
- claim-control checks
- case-page drafting
- copy options
- prompt writing
- visual-direction prompts
- image-generation direction
- QA checklists
- issue triage
- handoff prompts for implementation tools
- documentation discipline

This method must not decide:

- final design tokens
- final typography
- final colours
- final grid or spacing
- final component rules
- final case claims
- final public-use permissions
- legal text
- client/brand approval
- whether Phase 1 is done

---

## Working principle

AI may accelerate the work, but Mika's portfolio must remain evidence-based, visually controlled, and claim-safe.

AI output is useful when it helps to:

- clarify structure
- reduce chaos
- reveal risk
- draft alternatives
- compare options
- document decisions
- produce focused prompts
- support QA

AI output is harmful when it:

- invents client facts
- invents metrics
- invents roles or responsibilities
- creates generic portfolio language
- replaces visual judgment
- turns archive material into current truth
- over-polishes weak evidence
- makes conceptual work look like client work
- creates template, SaaS, shadcn, Material UI, neobrutalist, or AI-slop aesthetics

---

## Source hierarchy rule

AI must follow the current clean-source hierarchy.

Only current clean project files can act as active project truth.

Draft files can guide work but need Mika approval before becoming current.

Historical chats, old uploads, old screenshots, old prompts, archive material, and prior summaries are archive context only unless Mika explicitly reclassifies a specific item.

If a fact is missing, mark it as missing. Do not reconstruct it from memory.

---

## Claim-control method

Before any public-facing copy is accepted, check every claim against evidence.

### Claim levels

| Level | Meaning | Public use |
|---|---|---|
| Confirmed | Supported by current source or Mika-confirmed clean evidence | Can be used carefully |
| Draft / needs review | Exists in a draft source or working evidence but not approved as final | Use only as working copy |
| Working memory | Comes from previous chat, memory, or audit summary | Reconfirm or soften before use |
| Missing | No reliable source yet | Do not use publicly |
| Unsafe | Contradicts evidence or implies unsupported ownership/outcome | Remove |

### Blocked claim types

Do not invent:

- clients
- KPIs
- outcomes
- responsibilities
- research findings
- testing results
- testimonials
- awards
- campaign impact
- tools
- permissions
- NDA clearance
- launch status
- medical, therapeutic, or technical capabilities

---

## AI-use labels for portfolio work

When AI-assisted material is shown or discussed, label it accurately.

| Label | Meaning |
|---|---|
| `AI-assisted` | AI contributed to ideation, exploration, visual generation, copy drafting, or workflow support |
| `Prompted` | Prompting was a substantial part of output creation or exploration |
| `Curated` | AI or non-AI output was selected, edited, filtered, or directed through human judgment |
| `Remastered` | Existing material was improved or adapted for presentation |
| `Reconstructed` | A presentation asset was rebuilt because original material could not be shown or no longer exists |
| `Conceptual / Lab` | Speculative, self-initiated, educational, or experimental work |
| `Withheld` | Material exists but is not public because of rights, NDA, quality, or claim risk |

Use these labels to avoid pretending that reconstructed or AI-assisted material is original client production.

---

## Prompting standard

Prompts should be specific, visual, disciplined, and scoped to one task.

Good prompts define:

- goal
- audience
- context
- source constraints
- visual or editorial intent
- what must stay unchanged
- what must be avoided
- desired output format

Bad prompts:

- ask for generic polish
- ask AI to invent missing case details
- over-prescribe layout micro-details without design rationale
- produce decorative filler
- change things not mentioned
- create claims without source support

For Figma or builder prompts, end with:

> Do not change anything not mentioned in this prompt.

---

## Visual-generation method

AI-generated or AI-edited visuals may be used for exploration, concept development, remastering, or reconstruction, but not as fake evidence of real work.

Before a generated visual is used publicly, classify it as:

- Original
- Remastered
- Reconstructed
- Conceptual / Lab
- Anonymised
- Withheld
- Needs permission

AI visuals should be rejected if they show:

- generic AI gloss
- overused cinematic lighting
- incoherent typography
- fake UI details
- incorrect logos or brand assets
- misleading campaign evidence
- weak composition
- stock-like look
- decorative filler
- unlabelled reconstruction

---

## Case-writing method

Use this sequence for every case:

1. Confirm the case source exists.
2. Separate confirmed facts from working memory and missing information.
3. Define safe role wording.
4. Define unsafe claims to avoid.
5. Select visuals or screens only after asset review.
6. Write short website copy from evidence.
7. Run claim-control QA.
8. Run visual/seniority QA.
9. Keep unresolved questions visible.
10. Move non-blocking improvements to post-launch.

For Phase 1, cases do not need to be exhaustive. They need to be credible, visible, and sendable.

---

## Copy method

Website copy should be:

- English unless Mika confirms otherwise
- confident
- direct
- editorial
- precise
- evidence-based
- free of inflated generic claims

Avoid:

- passionate
- innovative
- out-of-the-box
- award-winning
- proven impact
- transformed
- fake seniority language
- unsupported business outcomes
- therapeutic, medical, or technical claims without proof

---

## QA method support

AI can support QA by checking:

- sendability
- claim risk
- content completeness
- design integrity
- mobile and desktop issues
- template/slop risk
- whether visible work is actually visible
- whether a page works for senior design decision-makers

AI QA is not final approval. Mika must confirm consequential launch decisions.

---

## Tool routing draft

No tool workflow is final unless Mika confirms it.

Suggested routing:

| Task | Possible tool / workflow | Risk |
|---|---|---|
| Strategy, source conflicts, architecture, positioning | Claude or ChatGPT | Can over-abstract if not grounded in current sources |
| Code, multi-file implementation, debugging, CSS/JS, Framer overrides | Codex or implementation tool | Can drift from design/source decisions if prompt is vague |
| Visual ideation, image remastering, reconstruction | image-generation tools | Can create misleading or generic visuals if not labelled |
| Source extraction, QA, claim-control | ChatGPT | Must cite or reference current sources, not memory |
| Figma adjustments | Figma / builder workflow | Must preserve unchanged areas and avoid generic defaults |

This table is advisory only.

---

## Handoff prompt structure

Use this structure when sending work to another tool:

```md
Task:

Context:

Current source of truth:

Do use:

Do not use:

What must stay unchanged:

Required output:

Acceptance criteria:

Do not change anything not mentioned in this prompt.
```

For code tasks, include file paths and expected behaviour.

For visual tasks, include art-direction intent, hierarchy, constraints, and what must be preserved.

For copy tasks, include evidence boundaries and unsafe claims.

---

## Open questions before this method becomes current

1. Which AI tools are approved for Phase 1 production support?
2. Which tools are exploration-only?
3. Which tools may touch final copy?
4. Which tools may touch final visuals?
5. Which tool should be used for implementation?
6. What counts as acceptable reconstruction for portfolio visuals?
7. How should AI-assisted or reconstructed material be labelled on the website?
8. Should an AI Practice page later document this method publicly?
9. Which parts of this workflow are Phase 1 critical and which are post-launch?
10. What is the final design-system source for visual decisions?

---

## Recommended next steps

1. Mika reviews this draft method.
2. Confirm which parts are approved for Phase 1.
3. Keep all unapproved tool workflows as advisory only.
4. Apply the method to Floom and CUPRA case-page drafting.
5. Revisit this file after the design-system source is confirmed.
6. Decide later whether this becomes public AI Practice content.

---

## Change log

| Date | Change |
|---|---|
| 2026-07-10 | v0.1 — Created draft AI workflow method source with source hierarchy, claim-control, prompting, visual-generation, case-writing, QA, and tool-routing rules |
