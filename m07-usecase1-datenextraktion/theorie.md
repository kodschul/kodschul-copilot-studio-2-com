# M07 Theorie: Use Case 1 — Datenextraktion aus Plänen

> Lesetext für die Teilnehmenden und Showcase-Vorlage für den Trainer. Trainer-Hinweise stehen
> gesammelt im Abschnitt "Trainer-Showcase".

## Lernziel

Nach diesem Modul habt ihr einen Agenten gebaut, der Flächen-/Mengendaten aus einem Plan extrahiert,
und kennt den Unterschied zwischen PDF- und DXF-Extraktion sowie deren Grenzen.

## Dauer

Tag 2 · 10:45–12:15 · 90 Minuten

## Ausgangslage

PDF-Pläne sind der Hauptfall bei EFG (häufigster, meist einzig verfügbarer Fall). DXF-Pläne sind der
Sonderfall — sie sind strukturierter und daher technisch einfacher auszulesen.

## Agent-Aufbau: Extraktions-Skill/Tool

1. Den Agenten (aus M06 oder neu) um ein Tool "Dokument/Plan einlesen" erweitern
2. Instruktionen ergänzen: "Extrahiere alle Flächen-/Mengenangaben aus dem Plan und gib sie als Tabelle
   mit Spalten Raum/Bauteil, Fläche, Einheit zurück"
3. Mit dem Beispiel-PDF-Plan testen, Ergebnis prüfen — [../musterdaten/beispiel-plan.pdf](../musterdaten/beispiel-plan.pdf)
4. Mit dem Beispiel-DXF-Plan testen, Unterschiede besprechen — [../musterdaten/beispiel-plan.dxf](../musterdaten/beispiel-plan.dxf)

→ Übung siehe [uebung.md](uebung.md).

## Strukturierte Ausgabe definieren

Ein gemeinsames Zielformat (Tabelle: Raum/Bauteil, Fläche, Einheit, Quelle/Plan-Referenz) ist die
Schnittstelle zu Power Automate in M08.

## Diskussion: Fehlerquellen und Erwartungsmanagement

Wo passieren heute die häufigsten Fehler bei m²-Angaben (Übertragungsfehler, Tippfehler, falsche
Zuordnung)? Bei reinen PDF-Plänen gilt: das Ergebnis ist eine **Arbeitserleichterung mit Prüfschritt**,
kein fehlerfreier Autopilot — dieses Erwartungsmanagement ist besonders gegenüber der Geschäftsleitung
wichtig.

## Trainer-Showcase

- **Ausgangslage (10 Min):** PDF- vs. DXF-Fall kurz gegenüberstellen, Prequestion stellen (siehe unten).
- **Agent-Aufbau (40 Min, Live + Nachbauen):** die 4 Schritte live vorführen, TN bauen parallel/danach
  in der Übung mit.
- **Strukturierte Ausgabe (15 Min):** Zielformat gemeinsam im Plenum festlegen.
- **Diskussion (15 Min):** offen über Grenzen sprechen, Erwartungsmanagement gegenüber der
  Geschäftsleitung betonen.
- **Prequestion (zu Beginn):** "Was glaubt ihr, wo wird die Extraktion bei reinen PDF-Plänen an
  Grenzen stoßen?" (z. B. Scanqualität, handschriftliche Vermaßung, uneinheitliche Layouts)

## Leitfragen

Beantwortet die Fragen zuerst selbst, bevor ihr sie aufklappt.

<details>
<summary>Warum liefert DXF tendenziell zuverlässigere Ergebnisse als PDF?</summary>

Weil die Daten in DXF strukturiert vorliegen (LINE-/TEXT-Entitäten), während PDF oft aus Rastertext
oder uneinheitlichem Layout besteht, das schwerer zuverlässig auszulesen ist.

</details>

<details>
<summary>Warum ist "Arbeitserleichterung mit Prüfschritt" die richtige Erwartungshaltung?</summary>

Weil Extraktionsergebnisse Fehler enthalten können (Halluzination, Datenqualität) — vor allem, bevor
sie automatisiert an Solarcomputer weitergegeben werden, müssen sie stichprobenartig geprüft werden.

</details>
