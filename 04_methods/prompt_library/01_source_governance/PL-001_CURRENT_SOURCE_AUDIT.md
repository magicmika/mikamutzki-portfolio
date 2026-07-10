# PL-001 — Current Source Audit

Status: draft  
Version: 0.1  
Category: Source Governance  
Primary tool: tool-agnostic; requires file-reading and long-context capability  
Test status: not yet tested in this library

---

## Purpose

Dieser Prompt prüft den aktuellen Projektstand, die aktive Quellenhierarchie, Konflikte, fehlende Blocker und den nächsten zulässigen Arbeitsschritt.

Er ist für Projektübernahmen, Clean Restarts, umfangreiche Wissensbasen und Situationen gedacht, in denen historische Dateien, aktuelle Quellen und unbestätigte Annahmen sauber getrennt werden müssen.

---

## When to use

- bei einem neuen Projekt-Setup
- nach einem größeren Quellen-Upload
- vor einer strategischen oder gestalterischen Entscheidung
- wenn mehrere Dateien unterschiedliche Aussagen enthalten
- wenn unklar ist, was aktuell, draft, historisch oder fehlend ist
- vor dem Schreiben von Case Copy oder Produktionsbriefings

---

## Required inputs

- aktive Projektdateien
- Source Map oder vergleichbares Quellenregister
- Baseline / Current State
- Definition of Done oder Projektziel
- optional: Evidence-, Method- und QA-Dateien
- optional: eine konkrete Frage oder geplante Produktionsaufgabe

---

## Source requirements

Mindestens eine Quelle muss den Status und die Autorität der übrigen Quellen definieren.

Historische Dateien dürfen nicht automatisch als Wahrheit behandelt werden.

Fehlende Informationen müssen als fehlend sichtbar bleiben.

---

## Variables

- `{{PROJECT_NAME}}`
- `{{PROJECT_GOAL}}`
- `{{SOURCE_HIERARCHY_FILE}}`
- `{{BASELINE_FILE}}`
- `{{DEFINITION_OF_DONE_FILE}}`
- `{{ACTIVE_FILES}}`
- `{{PLANNED_TASK}}`
- `{{LANGUAGE}}`

---

## Prompt

```text
You are auditing the current operational source state for {{PROJECT_NAME}}.

Project goal:
{{PROJECT_GOAL}}

Current source hierarchy:
{{SOURCE_HIERARCHY_FILE}}

Current baseline:
{{BASELINE_FILE}}

Definition of Done or release criteria:
{{DEFINITION_OF_DONE_FILE}}

Files to review:
{{ACTIVE_FILES}}

Planned next task:
{{PLANNED_TASK}}

Your task is to determine what is currently confirmed, what is only draft or advisory, what is historical, what is missing, and whether the planned next task is allowed by the current source state.

Rules:
- Use only the provided active sources.
- Do not use memory, previous chats, archived files, screenshots, or assumptions unless a current source explicitly reclassifies them.
- Do not convert draft material into current truth.
- Do not invent missing decisions, facts, assets, claims, permissions, tools, workflows, or design rules.
- If two current sources conflict, stop and identify the conflict.
- Distinguish project truth, evidence, method, task context, recommendation, and unresolved questions.
- Do not rewrite project files.
- Do not start design, copywriting, implementation, or production work.

Provide the result in {{LANGUAGE}} using exactly this structure:

# CURRENT SOURCE AUDIT

## 1. Confirmed current state
State only what is explicitly supported by current sources.

## 2. Source hierarchy
List the active authority order and explain what each source may decide.

## 3. Draft and advisory material
List draft or method sources and explain their limits.

## 4. Historical or excluded material
List sources that must not influence the project automatically.

## 5. Conflicts
List any contradictions between active sources. Write “None found” if none exist.

## 6. Missing blockers
List only missing information that genuinely blocks the planned task.

## 7. Planned task assessment
Rate the planned task as:
- ALLOWED
- ALLOWED WITH CONSTRAINTS
- BLOCKED

Explain why.

## 8. Exact next action
Name one concrete next action and the exact sources or files required.

## 9. One focused question
Ask only one question if a genuine blocker remains. Otherwise write “No question required.”
```

---

## Expected output

Ein kompakter Source Audit mit:

- bestätigtem Stand
- Autoritätsreihenfolge
- Draft-Grenzen
- Konflikten
- echten Blockern
- Bewertung des nächsten Arbeitsschritts
- einer klaren nächsten Aktion

---

## Acceptance criteria

- Keine historische Quelle wird als aktuell behandelt.
- Drafts werden nicht versehentlich freigegeben.
- Aussagen sind den richtigen Quellentypen zugeordnet.
- Konflikte werden klar benannt.
- Fehlende Informationen werden nicht rekonstruiert.
- Der nächste Schritt ist konkret und klein genug, um ausgeführt zu werden.
- Maximal eine Rückfrage wird gestellt.

---

## Risks and failure modes

- Das Modell fasst nur Dateien zusammen, statt Autorität und Konflikte zu prüfen.
- Drafts werden sprachlich wie bestätigte Wahrheit behandelt.
- Historische Informationen schleichen sich über allgemeines Modellwissen ein.
- Der Output enthält bereits neue Architektur-, Design- oder Copy-Entscheidungen.
- Zu viele Rückfragen blockieren die Arbeit.
- Der „nächste Schritt“ bleibt abstrakt.

---

## Do not use when

- nur eine einzelne, eindeutig bestätigte Datei zusammengefasst werden soll
- die Aufgabe bereits klar abgegrenzt und nicht source-kritisch ist
- eine Design-, Copy- oder Implementierungsleistung direkt benötigt wird

---

## Test notes

Noch nicht getestet. Erster realer Test sollte mit dem aktuellen Clean-Project-Repository erfolgen.

---

## Change log

| Date | Version | Change |
|---|---|---|
| 2026-07-10 | 0.1 | Initial library version |
