# PL-002 — Case Evidence Audit

Status: draft  
Version: 0.1  
Category: Case Studies  
Primary tool: tool-agnostic; requires multi-file analysis  
Test status: not yet tested in this library

---

## Purpose

Dieser Prompt prüft sämtliches verfügbares Material für eine Case Study, bevor Narrative, Website Copy oder visuelle Struktur entwickelt werden.

Er trennt bestätigte Fakten, Rollen, Assets, Outcomes, unsichere Erinnerungen, Widersprüche, Rechtefragen und unsafe Claims.

---

## When to use

- vor dem Schreiben einer Case Study
- vor dem Aufbau einer Case Page
- bei realen Kunden- oder Agenturprojekten
- bei konzeptionellen oder akademischen Projekten
- wenn Rollenverteilung oder Projektergebnisse unklar sind
- wenn Originalassets fehlen oder Rekonstruktionen erwogen werden

---

## Required inputs

- alle aktiven Case-Quellen
- Originalnachweise, sofern vorhanden
- Asset-Listen oder Projektdateien
- aktuelle Source Map
- gewünschter öffentlicher Kontext
- optional: bestehende Case-Hypothesen oder Arbeitstitel

---

## Source requirements

Originalnachweise und aktuelle Mika-bestätigte Fakten haben Vorrang.

Frühere Chats, Erinnerungen und Audits müssen als Working Memory oder Secondary Evidence gekennzeichnet werden, sofern sie nicht in der aktuellen Source Map freigegeben sind.

---

## Variables

- `{{CASE_NAME}}`
- `{{PROJECT_TYPE}}`
- `{{TARGET_AUDIENCE}}`
- `{{ACTIVE_CASE_SOURCES}}`
- `{{ORIGINAL_EVIDENCE}}`
- `{{ASSET_LOCATIONS}}`
- `{{WORKING_HYPOTHESES}}`
- `{{LANGUAGE}}`

---

## Prompt

```text
You are auditing all currently available evidence for the portfolio case {{CASE_NAME}}.

Project type:
{{PROJECT_TYPE}}

Target audience:
{{TARGET_AUDIENCE}}

Active case sources:
{{ACTIVE_CASE_SOURCES}}

Original evidence and proof:
{{ORIGINAL_EVIDENCE}}

Known asset locations:
{{ASSET_LOCATIONS}}

Working hypotheses or draft claims:
{{WORKING_HYPOTHESES}}

Your task is to build a claim-safe evidence audit before any final case narrative, website copy, visual selection, or page structure is created.

Rules:
- Use only the supplied current and explicitly allowed sources.
- Do not invent facts, dates, clients, roles, team structures, responsibilities, tools, deliverables, research findings, testing results, permissions, outcomes, KPIs, testimonials, awards, or impact.
- Separate direct evidence, Mika-confirmed information, working memory, inference, and missing information.
- Do not turn a polished hypothesis into a fact.
- Do not assume that an available asset is cleared for public use.
- Do not assume that a brand name, logo, client relationship, NDA status, or campaign image may be published.
- Distinguish original, remastered, reconstructed, anonymised, conceptual, withheld, and permission-pending material.
- Do not write final website copy.
- Do not decide the final case-page structure.
- Do not add generic UX or Art Direction process steps unless they are evidenced.

Provide the result in {{LANGUAGE}} using exactly this structure:

# CASE EVIDENCE AUDIT — {{CASE_NAME}}

## 1. Case classification
State whether the case is real client work, agency-side contribution, employment work, educational work, fictional concept, self-initiated work, conceptual work, or currently unclear.

## 2. Confirmed facts
List only facts directly supported by current evidence.

## 3. Mika-confirmed facts
List facts explicitly confirmed by Mika but not yet supported by original documents, if any.

## 4. Role and responsibility boundaries
Separate:
- supported contribution wording
- wording that needs softer framing
- wording that is currently unsafe

## 5. Available assets
For each asset or asset group, state:
- what exists
- source location
- review status
- public-use status
- recommended label

## 6. Process evidence
List documented process material and distinguish it from inferred process.

## 7. Outcomes and metrics
Separate:
- confirmed outcomes
- unverified outcomes
- missing outcomes
- claims that must not be used

## 8. Conflicts and ambiguities
List contradictions, unclear relationships, naming issues, timeline issues, or evidence gaps.

## 9. Unsafe claims
Provide a concise “Do not claim” list.

## 10. Phase 1 usable proof
List the minimum evidence that could credibly support a short Phase 1 case.

## 11. Missing blockers
List only the information or assets required before public publication.

## 12. Exact next evidence task
Name one concrete next task, the source needed, and the expected result.

Do not write final case copy.
```

---

## Expected output

Ein belastbares Case-Inventar, das später als Grundlage für Copy, Visual Selection, Page Architecture und Claim-Control dient.

---

## Acceptance criteria

- Projektart und Realitätsstatus sind klar.
- Mikas Rolle wird weder aufgebläht noch unklar gelassen.
- Assets und Rechte werden getrennt bewertet.
- Outcomes und KPIs werden nur mit Beleg zugelassen.
- Working Memory ist sichtbar markiert.
- Unsafe Claims sind explizit aufgeführt.
- Der Output enthält keine fertige Marketing-Narrative.
- Der nächste Evidence Task ist konkret.

---

## Risks and failure modes

- Das Modell schreibt bereits eine überzeugende Case Story.
- Unsichere Informationen werden durch elegante Sprache verschleiert.
- „Contributed to“ wird zu „led“ oder „owned“ aufgebläht.
- Fehlende Originalassets werden als vorhanden dargestellt.
- Rechte- und NDA-Fragen werden ignoriert.
- Generische Designprozess-Schritte werden ergänzt, obwohl sie nicht dokumentiert sind.
- Educational oder fictional work wird wie ein reales Kundenprodukt dargestellt.

---

## Do not use when

- alle Case-Fakten und Assets bereits vollständig bestätigt sind
- nur eine konkrete Copy-Variante benötigt wird
- die Aufgabe ausschließlich visuelle QA betrifft

---

## Test notes

Noch nicht getestet. Erste Tests: Floom und CUPRA.

---

## Change log

| Date | Version | Change |
|---|---|---|
| 2026-07-10 | 0.1 | Initial library version |
