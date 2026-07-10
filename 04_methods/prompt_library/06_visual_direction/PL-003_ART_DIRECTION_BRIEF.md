# PL-003 — Art Direction Brief

Status: draft  
Version: 0.1  
Category: Visual Direction  
Primary tool: tool-agnostic; suitable for image, layout, Figma, builder or production handoff  
Test status: not yet tested in this library

---

## Purpose

Dieser Prompt übersetzt eine visuelle Aufgabe in einen präzisen Art-Direction-Brief.

Er beschreibt nicht nur Objekte und Layoutpositionen, sondern Zielwirkung, visuelle Spannung, Hierarchie, Rhythmus, Materialität, Bildlogik, Kontext und Qualitätsgrenzen.

---

## When to use

- für Hero Visuals
- für Editorial Layouts
- für Case-Study-Medienmodule
- für Image Generation oder Image Editing
- für Figma- oder Builder-Handoffs
- für Remastering oder Reconstruction
- wenn ein Output technisch korrekt, aber visuell generisch ist
- wenn Seniorität, visuelle Kontrolle oder Eigenständigkeit fehlen

---

## Required inputs

- Aufgabe und Ziel
- Zielgruppe
- Einsatzort und Format
- aktuelle Quellen oder Assets
- was bereits funktioniert
- was verändert werden muss
- visuelle Referenzen oder beschriebene Prinzipien
- technische Constraints
- verbotene Stilrichtungen oder Elemente

---

## Source requirements

Bestehende bestätigte Assets und Gestaltungsentscheidungen müssen benannt werden.

Historische oder unbestätigte Designrichtungen dürfen nicht automatisch übernommen werden.

Rekonstruktionen und AI-generierte Assets müssen als solche gekennzeichnet werden.

---

## Variables

- `{{TASK}}`
- `{{CONTEXT}}`
- `{{AUDIENCE}}`
- `{{PLACEMENT_AND_FORMAT}}`
- `{{CURRENT_ASSETS}}`
- `{{PRESERVE}}`
- `{{CHANGE}}`
- `{{DESIRED_EFFECT}}`
- `{{VISUAL_PRINCIPLES}}`
- `{{MATERIAL_AND_IMAGE_LOGIC}}`
- `{{HIERARCHY_AND_RHYTHM}}`
- `{{CONSTRAINTS}}`
- `{{AVOID}}`
- `{{OUTPUT_FORMAT}}`

---

## Prompt

```text
Act as a senior Art Director working on {{TASK}}.

Context:
{{CONTEXT}}

Audience:
{{AUDIENCE}}

Placement and format:
{{PLACEMENT_AND_FORMAT}}

Current assets or source material:
{{CURRENT_ASSETS}}

Preserve:
{{PRESERVE}}

Change:
{{CHANGE}}

Desired effect:
{{DESIRED_EFFECT}}

Visual principles:
{{VISUAL_PRINCIPLES}}

Material and image logic:
{{MATERIAL_AND_IMAGE_LOGIC}}

Hierarchy and rhythm:
{{HIERARCHY_AND_RHYTHM}}

Constraints:
{{CONSTRAINTS}}

Avoid:
{{AVOID}}

Create a precise production-ready Art Direction brief.

The brief must:
- define the intended first impression
- explain the visual hierarchy
- describe composition, tension, rhythm, scale and focal control
- describe image treatment, materiality, lighting, contrast and spatial logic where relevant
- explain how the work should support the content instead of decorating it
- identify what must remain unchanged
- identify the strongest quality risks
- provide clear acceptance criteria
- avoid generic design language such as “modern”, “clean”, “premium”, “bold” or “innovative” unless each term is made visually specific
- avoid generic SaaS, startup-template, shadcn, Material UI, neobrutalist or AI-gloss aesthetics
- avoid inventing brand assets, typography, colours, components, claims or content
- distinguish original, remastered, reconstructed and conceptual material where relevant

Return the result in this structure:

# ART DIRECTION BRIEF

## 1. Objective
## 2. Intended first impression
## 3. Core visual idea
## 4. Composition and spatial logic
## 5. Hierarchy and rhythm
## 6. Image treatment and materiality
## 7. Typography and graphic behaviour
Only describe typography if a confirmed type source exists. Otherwise mark it as open.

## 8. Interaction or motion behaviour
Only include this section when relevant.

## 9. Preserve
## 10. Change
## 11. Avoid
## 12. Acceptance criteria
## 13. Quality risks
## 14. Production notes

Output format:
{{OUTPUT_FORMAT}}
```

---

## Expected output

Ein Art-Direction-Brief, der als Grundlage für ein eng begrenztes visuelles Produktionsprompt, einen Figma-Handoff oder eine manuelle Designentscheidung dienen kann.

---

## Acceptance criteria

- Zielwirkung und erste Wahrnehmung sind konkret beschrieben.
- Der Brief benennt Hierarchie, Rhythmus und Fokus.
- Visuelle Begriffe sind nicht generisch.
- Bestehende starke Elemente werden geschützt.
- Unbestätigte Designsystemwerte werden nicht erfunden.
- Decorative filler und AI-Slop werden ausdrücklich ausgeschlossen.
- Der Brief kann in einen kleineren Produktionsprompt überführt werden.
- Acceptance Criteria sind visuell überprüfbar.

---

## Risks and failure modes

- Der Output bleibt bei Adjektiven wie „modern“ und „premium“ stehen.
- Der Brief beschreibt nur Objekte, aber keine Wirkung.
- Zu viele Stilreferenzen erzeugen eine inkohärente Mischung.
- Bestehende starke Elemente werden versehentlich neu interpretiert.
- Unbestätigte Farben, Fonts oder Komponenten werden erfunden.
- Der Brief wird zu lang und ist nicht mehr produktionsfähig.
- Das Modell formuliert bereits ein finales Image-Generation-Prompt, obwohl erst die Richtung geklärt werden sollte.

---

## Do not use when

- nur ein technischer Größen-, Export- oder Formatfehler korrigiert werden soll
- die visuelle Richtung bereits vollständig bestätigt ist und nur eine minimale Korrektur benötigt wird
- keine Assets, kein Kontext und keine Zielwirkung vorliegen

---

## Test notes

Noch nicht getestet. Erste Tests sollten mit einem konkreten Portfolio-Hero oder einem Case-Media-Modul erfolgen.

---

## Change log

| Date | Version | Change |
|---|---|---|
| 2026-07-10 | 0.1 | Initial library version |
