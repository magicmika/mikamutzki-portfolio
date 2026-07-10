# 10_AI_WORKFLOW_METHOD

Stand: 10. Juli 2026  
Status: Arbeitsversion für Phase 1

## Zweck

Dieses Dokument beschreibt die operative AI-Workflow-Methode für das Portfolio-Projekt. Es legt keine neuen Produktversprechen, keine finalen Tool-Claims und keine neue Design-Authority fest. Es definiert, wie AI im Projekt **gezielt**, begrenzt, überprüfbar und ohne AI-Slop eingesetzt wird.[cite:15][cite:19]

Die Methode basiert auf drei Ebenen: erstens klarer Source Governance, zweitens kontrollierter Tool-Rollen, drittens wiederholbaren Qualitäts- und Entscheidungsregeln. Die Datei ist bewusst praxisnah formuliert, damit sie im Alltag nutzbar bleibt und nicht nur strategisch gut klingt.[cite:15][cite:19]

## Geltungsbereich

Diese Methode gilt für Recherche, Struktur, Copy, visuelle Exploration, Asset-Produktion, Vibe-Coding, QA und Dokumentation im Projekt MIKAMUTZKI — FINAL PORTFOLIO. Figma bleibt Design Authority; aktuelle Projektdateien bleiben Source of Truth; Mika bleibt die letzte inhaltliche und gestalterische Entscheidungsinstanz.[cite:15][cite:19]

Das Dokument entscheidet nicht über finale Website-Architektur, finale Tokens, finale öffentliche Claims oder einen endgültig festgelegten Build-Stack. Solche Entscheidungen werden nur auf Basis bestätigter Projektquellen, realer Tests und expliziter Freigaben getroffen.[cite:19]

## Arbeitsprinzipien

### 1. System First

Kein Screen, Asset, Textblock oder Build-Schritt startet ohne klaren Rahmen. Dazu gehören Ziel, Quelle, Scope, Ausschlüsse, Qualitätskriterien und die zuständige Entscheidungsinstanz.[cite:19]

AI wird nicht verwendet, um Unklarheit zu kaschieren. Wenn Struktur, Hierarchie oder Beleglage unklar sind, wird zuerst die Grundlage geklärt und erst danach erzeugt.[cite:19]

### 2. One authority per decision

Für jede Entscheidung gibt es genau eine Autorität. Figma entscheidet Gestaltung, bestätigte Quellen entscheiden Fakten, Mika entscheidet Freigabe und Veröffentlichung.[cite:19]

Mehrere Tools dürfen Input liefern, aber kein Tool darf durch Wiederholung oder Selbstsicherheit eine unbestätigte Behauptung aufwerten. Drei ähnliche Outputs sind noch keine Wahrheit.[cite:19]

### 3. Generate narrowly, review broadly

Erzeugung bleibt eng begrenzt. Prüfung bleibt breit. Das reduziert Modell-Drift, unnötige Varianten und versteckte Nebenwirkungen.[cite:19]

Statt offene Mega-Prompts zu schreiben, werden Aufgaben in kleine, prüfbare Schritte zerlegt: Struktur, Richtung, Variante, Auswahl, Härtung, QA. Das passt auch zu den dokumentierten Modell- und Tool-Grenzen in visuellen und generativen Workflows.[cite:15][cite:17][cite:19]

### 4. Preserve what works

Jede Änderung schützt bestätigte Inhalte, funktionierende Gestaltung und bereits geprüfte Komponenten. Korrektur bedeutet nicht automatischen Neuaufbau.[cite:19]

Wenn ein Output bereits tragfähig ist, wird verfeinert statt neu erfunden. Diese Regel schützt das Projekt vor Builder-Drift, unnötigem Stilwechsel und AI-Slop.[cite:15][cite:19]

### 5. Stop after two failed correction loops

Wenn zwei enge Korrekturschleifen kein sauberes Ergebnis liefern, wird nicht weiter im selben Muster gepromptet. Dann wird die Fehlerklasse bestimmt: Source, Strategy, Art Direction, Prompt, Tool, Implementation, QA oder Scope.[cite:19]

Danach wird Task, Prompt oder Tool gewechselt – oder manuell gelöst. Diese Regel ist wichtig, weil viele schlechte AI-Schleifen nicht am Talent des Nutzers scheitern, sondern an falscher Werkzeugwahl oder zu großem Scope.[cite:19]

## Workflow-Reihenfolge

### 1. Source Governance

Vor jeder Arbeit wird geprüft: Was ist aktuelle Wahrheit, was ist Kontext, was ist Hypothese? Aktuelle Projektdateien und bestätigte Entscheidungen haben Vorrang vor alten Chats, alten Uploads oder Modellzusammenfassungen.[cite:19]

Alles, was öffentlich behauptet werden könnte, braucht eine bestätigte Quelle. Unklare Punkte werden markiert, nicht geglättet.[cite:19]

### 2. Research und Synthese

Für Deep Research dürfen mehrere Modelle als Challenger eingesetzt werden. Die Recherche ist aber erst abgeschlossen, wenn Widersprüche sichtbar gemacht, Risiken benannt und Restunsicherheiten dokumentiert sind.[cite:19]

Dafür gilt der Claim-Ledger-Grundsatz: nicht nur „was wurde empfohlen“, sondern auch „wie belastbar ist die Aussage, welche Quelle trägt sie, wie hoch ist die Konfidenz und was ist das Abbruchkriterium“.[cite:19]

### 3. Strategie und Content Architecture

ChatGPT und Claude sind in dieser Methode primär für Struktur, Argumentation, Storyline, Gegenprüfung und Copy-Kritik gedacht. Sie sind nicht die Quelle für finale öffentliche Claims, wenn diese nicht durch Projektmaterial gedeckt sind.[cite:19]

Texte entstehen aus Evidence Notes, klarer Absatzfunktion und einer Specificity-Prüfung. Jeder Satz muss konkret, belegbar und für das Projekt notwendig sein.[cite:19]

### 4. Design Authority und visuelle Exploration

Figma bleibt der Ort, an dem Gestaltung entschieden und gehärtet wird. Explorationstools dürfen Richtungen, Varianten und Kompositionsideen liefern, aber keine neue Wahrheit über das Designsystem erzeugen.[cite:19]

Stitch, Claude Design oder ähnliche Tools sind deshalb Explorations- und Verfeinerungswerkzeuge, keine Ersatz-Autorität für Komponenten, Tokens oder finale UX-Entscheidungen.[cite:19]

### 5. Asset-Produktion

Visuelle Assets werden als Pipeline gedacht, nicht als Einzeltreffer. Das heißt: Auswahl des richtigen Werkzeugs, kleines Set von Varianten, Vergleich im Kontaktbogen, Auswahl, Retusche, Export.[cite:15][cite:19]

Kittl eignet sich für designnahe, redaktionelle und typografische Bildproduktion; Magnific eignet sich für dokumentierte Modellwahl, Bildgenerierung, Variation und Upscaling je nach Zielbild.[cite:15][cite:17][cite:18][cite:23]

### 6. Vibe Coding und Implementation

Code-Unterstützung ist in dieser Methode kontrolliert und slices-basiert. Es werden nur kleine, klar definierte Ausschnitte getestet, mit Preserve-Regeln, Akzeptanzkriterien und Diff-Prüfung.[cite:19]

AI-generierter Code darf nie stillschweigend Design- oder Content-Entscheidungen überschreiben. Semantisches HTML, klare Komponentenstruktur, definierte Breakpoints und Tastaturbedienung gehören zur Mindestprüfung.[cite:19]

### 7. QA und Dokumentation

QA ist kein Nachgedanke. Visuelle Qualität, State Coverage, Responsiveness, Lesbarkeit, Claim Control und Disclosure gehören zum Abschluss jedes relevanten Arbeitsschritts.[cite:15][cite:19]

Dokumentation ist Teil des Kompetenznachweises. Relevante Prompts, Entscheidungen, Fehlversuche, Diffs, Fixes und begrenzte Tool-Rollen werden kuratiert festgehalten.[cite:19]

## Modellauswahl bei Bildtools

### Grundregel

Nicht vom Modellnamen ausgehen, sondern vom Einsatzzweck. Die Auswahl beginnt immer mit drei Fragen: Brauche ich Typografie im Bild? Brauche ich Konsistenz über mehrere Assets? Brauche ich erst einmal nur eine schnelle Richtung?[cite:15][cite:17][cite:18][cite:19][cite:29][cite:30][cite:36]

Wenn diese drei Fragen nicht beantwortet sind, wird fast immer das falsche Modell gewählt. Das führt zu Credit-Verlust, unnötigen Iterationen und scheinbar „schlechtem“ AI-Output, obwohl das Problem oft nur eine falsche Modellklasse ist.[cite:15][cite:17][cite:19]

### Modellwahl-Heuristik

| Bedarf | Empfohlene Richtung | Begründung |
|---|---|---|
| Erste Richtung, wenig Risiko, schneller Start | Auto / Fast / kleine Standardmodelle | Gut für frühe Exploration, spart Credits und verhindert Overkill.[cite:15][cite:17] |
| Starke Typografie oder Text im Bild | Textstarke Modelle wie Ideogram 3 oder GPT Image 2 in Magnific; in Canva eher stil- und layoutorientiert arbeiten statt perfekte Text-Assets zu erwarten | Magnific nennt Ideogram 3 und GPT Image 2 explizit für präzise Textwiedergabe.[cite:15] |
| Konsistente Serie über mehrere Assets | Konsistenz-orientierte Modelle wie Nano Banana Pro oder Flux.2 Pro in Magnific; in Kittl mit festem Stil und wenigen Variablen arbeiten | Magnific beschreibt diese Modelle als stark für Konsistenz und Referenztreue.[cite:15] |
| Editorial, Case Header, kontrollierte Fotologik | Cinematic oder vergleichbare fotorealistische Modelle | Magnific beschreibt Cinematic als geeignet für studioartige, filmische Kompositionen.[cite:15] |
| Designnahe Komposition, Poster, strukturierte Visuals | Recraft V4 Pro oder Kittl mit passendem Style-Preset | Recraft wird in Magnific als designorientiertes Modell geführt; Kittl empfiehlt zuerst Style und dann Modellwahl.[cite:15][cite:18][cite:19] |
| Canva-Alltag, schnelle Bilder in Layout-Kontext | Magic Media oder Dream Lab mit passendem Style und Format; externe Modelle nur bei klarer Qualitätslücke | Canva positioniert seine Bildtools stark über Stil- und Formatwahl, nicht über tiefe Modellsteuerung.[cite:29][cite:30][cite:36] |

### Kittl-Regel

In Kittl wird zuerst über Style, Komposition und Designabsicht gearbeitet, nicht über Modellnamen allein. Kittl beschreibt die Bildgenerierung ausdrücklich als Prozess aus Prompt, Style, Modell und Settings, und Tutorials aus dem Kittl-Umfeld zeigen, dass Style-Presets oft der praktischere Einstieg sind als direkte Modellfixierung.[cite:18][cite:19][cite:22][cite:23]

Für dieses Portfolio heißt das: Kittl zuerst einsetzen, wenn typografische, redaktionelle oder präsentationsnahe Visuals entstehen sollen. Nur wenn die Aufgabe technisch enger ist – etwa Texttreue, extreme Konsistenz oder spezielle Lichtlogik – wird die Modellwahl bewusst enger geführt.[cite:18][cite:19][cite:23]

### Magnific-Regel

Magnific eignet sich besser als Kittl, wenn die Modellwahl selbst Teil der Qualitätssteuerung ist. Die offiziellen Dokumentationen unterscheiden dort klar nach Bildgenerator-Modellen, Upscaler-Engines, Variationsmodi und Credits.[cite:15][cite:17]

Für dieses Projekt ist Magnific deshalb kein „alles damit machen“-Tool, sondern ein gezieltes Werkzeug für drei Fälle: kontrollierte Modellwahl, selektive High-End-Variationen und punktuelle Veredelung bereits guter Assets. Es sollte nicht die erste Station jeder Bildidee sein.[cite:15][cite:17]

### Canva-Regel

Canva ist stark, wenn das Bild direkt im Layout- oder Kommunikationskontext entsteht. Canva stellt die Bildgenerierung vor allem über Stil, Seitenverhältnis, Generator-App und anschließende Layout-Nutzung dar; es ist weniger ein tiefes Modellwahl-Tool als ein schnelles Design-System-Umfeld für Bildproduktion im Editor.[cite:29][cite:30][cite:36][cite:40]

Für dieses Projekt heißt das: Canva eignet sich für schnelle Konzeptbilder, Kommunikationsgrafiken und Mockup-nahe Layoutkontexte. Wenn präzise Texttreue, Serienkonsistenz oder hochwertige Editorial-Bildwirkung entscheidend sind, sollte die Auswahl eher in Kittl oder Magnific stattfinden.[cite:29][cite:30][cite:36][cite:38]

## Anti-Slop-Regeln

### Copy

Kein generisches Portfolio-Vokabular ohne Beleg. Aussagen wie „passionate“, „innovative“, „meaningful experiences“ oder „from concept to execution“ werden markiert, nicht automatisch verwendet.[cite:19]

Jeder Absatz braucht genau einen Zweck. Stil darf die Beweislage nie künstlich verstärken.[cite:19]

### Visuals

Jedes visuelle Element braucht eine Funktion. Generische SaaS-Karten, Builder-Hausästhetik, übernutzte Pills, Soft-Gradient-Heroes, unnötige Dividers und rein dekorative Motion gelten als Risikomuster.[cite:19]

Visuals werden nie einzeln beurteilt, sondern mindestens in kleinen Sets verglichen. So werden Wiederholung, Modell-Hausstil und schwache Ausreißer sichtbar.[cite:19]

### Claims

Keine erfundenen KPIs, Rollen, Verantwortlichkeiten, Outcomes, Testimonials oder Produktfähigkeiten. Unklare Aussagen werden entweder belegt, abgeschwächt oder gestrichen.[cite:19]

Wenn eine Tool-Behauptung nur aus Modellrecherche stammt, aber nicht im Projekt verifiziert ist, bleibt sie Watchlist oder Testkandidat – nicht finaler Methodenbestandteil.[cite:19]

## Recovery-Protokoll

Wenn ein Ergebnis schlecht ist, wird nicht sofort alles umgeworfen. Erst wird das Symptom präzise beschrieben, dann die Fehlerklasse bestimmt, dann der kleinste prüfbare Test gewählt.[cite:19]

Die Reihenfolge lautet: Freeze, Symptom beschreiben, Fehlerklasse bestimmen, Scope verkleinern, Test neu aufsetzen, nach zwei Schleifen Tool oder Methode wechseln. Das hält die Arbeit ruhig, nachvollziehbar und sendbar.[cite:19]

## Qualitätsgates

Ein Ergebnis ist erst freigabefähig, wenn folgende Fragen sauber beantwortet sind:

- Ist die Aussage oder Gestaltung auf aktuelle Projektquellen rückführbar?[cite:19]
- Wurde nichts erfunden oder unnötig verstärkt?[cite:19]
- Ist die Gestaltung klar, hierarchisch und frei von Template-Risiko?[cite:19]
- Funktioniert das Ergebnis auch ohne Mockup-Inszenierung?[cite:19]
- Ist die Tool-Wahl dokumentiert und war sie für den Zweck angemessen?[cite:15][cite:17][cite:19]
- Wurde bei Bildtools das Modell nach Zweck statt nach Namen gewählt?[cite:15][cite:17][cite:18][cite:29][cite:30][cite:36]

## Einsatz im Projekt

Für Phase 1 unterstützt diese Methode ein sendbares Senior-Portfolio mit realer Arbeit online. Sie soll weder neue Komplexität erzeugen noch ein AI-lastiges Markenbild nach außen aufbauen.[cite:19]

Die Methode zeigt Seniorität nicht durch maximale Automatisierung, sondern durch Auswahl, Begrenzung, Kritik, Reparatur und dokumentierte Urteilsfähigkeit. Genau darin liegt ihr Wert für das Portfolio-Projekt.[cite:19]
