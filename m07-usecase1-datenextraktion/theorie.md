# M07 Theorie: Use Case 1 — Datenextraktion aus Plänen

## Lernziel

Einen Agenten bauen, der Flächen-/Mengendaten aus einem Plan extrahiert; Unterschied PDF vs. DXF und
dessen Grenzen kennen.

## Dauer

Tag 2 · 10:45–12:15 · 90 Minuten

## Ausgangslage (10 Min)

PDF-Pläne = Hauptfall bei EFG (häufigster, meist einzig verfügbarer Fall). DXF-Pläne = Sonderfall,
strukturierter und daher technisch einfacher auszulesen.

## Agent-Aufbau: Extraktions-Skill/Tool (40 Min, Live + Nachbauen)

1. Neuen Agenten (oder bestehenden aus M06) um ein Tool "Dokument/Plan einlesen" erweitern
2. Instruktionen ergänzen: "Extrahiere alle Flächen-/Mengenangaben aus dem Plan und gib sie als Tabelle
   mit Spalten Raum/Bauteil, Fläche, Einheit zurück"
3. Mit Beispiel-PDF-Plan testen, Ergebnis prüfen — [../musterdaten/beispiel-plan.pdf](../musterdaten/beispiel-plan.pdf)
4. Mit Beispiel-DXF-Plan testen, Unterschiede besprechen — [../musterdaten/beispiel-plan.dxf](../musterdaten/beispiel-plan.dxf)

→ Übung siehe [uebung.md](uebung.md).

## Strukturierte Ausgabe definieren (15 Min)

Gemeinsames Zielformat festlegen (Tabelle: Raum/Bauteil, Fläche, Einheit, Quelle/Plan-Referenz) — das
ist die Schnittstelle zu Power Automate in M08.

## Diskussion (15 Min)

Reduktion manueller Fehlerquellen: wo passieren heute die häufigsten Fehler bei m²-Angaben? Grenzen bei
reinen PDF-Plänen offen ansprechen: Ergebnis ist eine **Arbeitserleichterung mit Prüfschritt**, kein
fehlerfreier Autopilot — wichtig gegenüber der Geschäftsleitung im Raum.

## Leitfragen

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
