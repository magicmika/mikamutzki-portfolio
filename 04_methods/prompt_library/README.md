# MIKAMUTZKI Prompt Library

Version: 0.1  
Status: internal working library  
Project: MIKAMUTZKI — FINAL PORTFOLIO  
Language model: Prompt templates in English; documentation, use notes and risks in German

---

## Zweck

Diese Bibliothek sammelt keine zufälligen „guten Prompts“. Sie dokumentiert wiederverwendbare, überprüfbare Arbeitsabläufe für AI-assisted Research, Source Governance, Case Studies, Claim Control, Copy, Art Direction, Visual Production, Implementation und QA.

Sie verfolgt zwei Ziele:

1. **Operative Nutzung:** Prompts sollen echte Aufgaben im Portfolio-Projekt zuverlässig unterstützen.
2. **Kompetenznachweis:** Die Bibliothek soll später zeigen, dass Mika mit strukturierten AI-Workflows, klaren Quellenregeln, Acceptance Criteria, Risikoabwägung und dokumentierter Qualitätssicherung arbeitet.

---

## Sprachregel

- **Prompt Templates:** English
- **Dokumentation, Einsatzhinweise und Risiken:** German
- **Öffentliche Showcase-Auszüge:** später in English

---

## Bibliotheksprinzipien

### 1. Ein Prompt, eine Aufgabe

Jeder Prompt hat einen klar abgegrenzten Zweck. Große Aufgaben werden in überprüfbare Einzelschritte zerlegt.

### 2. Quellen vor Output

Kein Prompt darf fehlende Fakten, Rollen, Ergebnisse, Tools, Freigaben oder Designentscheidungen erfinden.

### 3. Prompt und Methode trennen

Die Dokumentation erklärt, wann und warum ein Prompt eingesetzt wird. Das eigentliche Prompt Template bleibt kopierbar und tooltauglich.

### 4. Acceptance Criteria verpflichtend

Ein Prompt ist nicht fertig, wenn er nur „gut klingt“. Das erwartete Ergebnis muss gegen klare Kriterien geprüft werden.

### 5. Risiken sichtbar halten

Jede Prompt-Datei nennt typische Failure Modes, ungeeignete Einsatzfälle und offene Testfragen.

### 6. Tool-neutral starten

Prompts werden zunächst möglichst tool-agnostisch formuliert. Tool-spezifische Varianten entstehen erst nach realen Tests.

### 7. Keine Rohprompts aus Kursmaterial

Kurs-PDFs, Beispiele und alte Prompts sind methodische Rohquellen. Sie werden nicht ungeprüft übernommen.

---

## Dateistruktur

```text
prompt_library/
  README.md
  00_PROMPT_INDEX.md
  01_source_governance/
    PL-001_CURRENT_SOURCE_AUDIT.md
  04_case_studies/
    PL-002_CASE_EVIDENCE_AUDIT.md
  06_visual_direction/
    PL-003_ART_DIRECTION_BRIEF.md
```

Weitere Kategorien werden erst ergänzt, wenn reale Aufgaben dafür existieren.

---

## Standard für jede Prompt-Datei

```text
# PL-XXX — Prompt Name

Status:
Version:
Category:
Primary tool:
Test status:

## Purpose
## When to use
## Required inputs
## Source requirements
## Variables
## Prompt
## Expected output
## Acceptance criteria
## Risks and failure modes
## Do not use when
## Test notes
## Change log
```

---

## Statuswerte

| Status | Bedeutung |
|---|---|
| `draft` | angelegt, aber noch nicht ausreichend getestet |
| `tested` | mindestens einmal erfolgreich an realem Material getestet |
| `stable` | mehrfach erfolgreich eingesetzt und dokumentiert |
| `deprecated` | nicht mehr verwenden |
| `archive` | nur historischer Kontext |

---

## Testprotokoll

Nach jedem realen Einsatz sollten mindestens diese Punkte dokumentiert werden:

- verwendetes Tool / Modell
- Datum
- Input-Typen
- Ergebnisqualität
- gefundene Fehler
- notwendige Korrekturen
- überarbeitete Prompt-Version
- Entscheidung: draft / tested / stable

---

## Aktueller Umfang v0.1

- PL-001 — Current Source Audit
- PL-002 — Case Evidence Audit
- PL-003 — Art Direction Brief

Die Bibliothek wird erst erweitert, wenn diese drei Prompts an echten Portfolio-Aufgaben getestet wurden.
