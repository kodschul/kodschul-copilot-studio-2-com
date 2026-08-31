# M00 Kursueberblick: KI-Agenten mit Microsoft Copilot Studio & Power Automate (EFG)

## Worum geht es in diesem Training?

Dieses 2-tägige Training befähigt die Teilnehmenden von EFG Engineering Facility Group
Ingenieurgesellschaft mbH dazu, mit Microsoft Copilot Studio eigene Agenten zu bauen und mit
Power Automate zu automatisieren — zugeschnitten auf zwei konkrete EFG-Anwendungsfälle:
Datenextraktion aus Plänen (PDF/DXF) Richtung Solarcomputer und Aufmaßprüfung (Soll/Ist-Abgleich).

Alle Eckdaten (Termin, Teilnehmer, Software-Umgebung) stehen in [00-eckdaten.md](../00-eckdaten.md),
der volle Zeitplan in [01-agenda.md](../01-agenda.md).

## Die zehn Module auf einen Blick

| #   | Modul | Tag | Kernergebnis |
| --- | --- | --- | --- |
| M01 | Auftakt, KI-Landschaft & Einführungsstrategie | Tag 1 | ChatGPT/Claude/Copilot eingeordnet, Einführungsoptionen bewertet |
| M02 | Grundlagen KI-Agenten | Tag 1 | Agent/Skill/Prompt definiert, erste Prompt-Übung |
| M03 | Copilot Studio im Überblick | Tag 1 | Aufbau eines Agenten verstanden |
| M04 | Power Platform im Überblick | Tag 1 | Power Automate Grundbausteine verstanden |
| M05 | Use-Case-Discovery Workshop | Tag 1 | Discovery-Canvas für beide EFG-Use-Cases |
| M06 | Recap & Aufbau eines einfachen Agenten | Tag 2 | Erster eigener Agent |
| M07 | Use Case 1: Datenextraktion aus Plänen | Tag 2 | Extraktions-Agent für Pläne |
| M08 | Automatisierung mit Power Automate | Tag 2 | Flow zur Datenübergabe |
| M09 | Use Case 2: Aufmaßprüfung | Tag 2 | Konzept-Skizze Prüf-Agent |
| M10 | Wrap-up, Erweiterung & Übergabe | Tag 2 | Nächste Schritte, Übergabe |

## Durchgängiges Beispielprojekt

Alle Übungen bauen auf denselben zwei EFG-Use-Cases auf:

- **Datenextraktion aus Plänen (PDF/DXF) → Solarcomputer:** Flächen-/Mengendaten aus Grundrissplänen
  extrahieren und ins Heizlastprogramm übernehmen.
- **Aufmaßprüfung:** Massenaufstellungen gegen Pläne prüfen (Soll/Ist-Abgleich).

Da keine echten EFG-Plandaten vorliegen, werden synthetische Musterdaten verwendet (siehe
[musterdaten/](../musterdaten/): beispiel-plan.pdf, beispiel-plan.dxf, massenaufstellung.csv).

## Trainingsregeln und Arbeitsweise

- Jedes Modul enthält mindestens eine Interaktion (Prequestion, Quiz, Übung oder Selbstreflexion) —
  Details siehe [best-practices.md](best-practices.md) und die didaktische Begründung in [trainer-guide.md](../trainer-guide.md).
- Offene Fragen (z. B. Solarcomputer-Connector) werden gesammelt und vor Ort mit dem Kunden geklärt.
- Ergebnisse aus den Übungen werden direkt im gebauten Agenten sichtbar (Testfenster).

## Deliverables am Trainingsende

1. Selbst gebauter Extraktions-Agent (Modul 7) inkl. Power-Automate-Flow (Modul 8)
2. Konzept-Skizze für den Aufmaßprüfungs-Agenten (Modul 9)
3. Ausgefüllte Discovery-Canvas für beide Use Cases (Modul 5)
4. Handout ([handout.md](../handout.md)) mit Glossar und Kernkonzepten
