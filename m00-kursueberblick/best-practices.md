# Best Practices: KI-Agenten mit Microsoft Copilot Studio & Power Automate (EFG)

Bewährte Prinzipien für Planung, Umsetzung und Betrieb der EFG-Agenten. Ergänzt die didaktischen
Grundlagen in [trainer-guide.md](../trainer-guide.md) ("Didaktisches Konzept: Interaktionen").

---

## Planung und Use-Case-Auswahl

**Problem vor Technologie**
Beide EFG-Use-Cases starten bei einem konkreten, wiederkehrenden Medienbruch (Plan → Solarcomputer,
Massenaufstellung → Plan), nicht bei der Technologie. Das erhöht die Erfolgswahrscheinlichkeit.

**Erwartungsmanagement von Anfang an**
Ein Extraktions-Agent ist eine Arbeitserleichterung mit Prüfschritt, kein fehlerfreier Autopilot.
Das gilt besonders gegenüber der Geschäftsleitung — realistische Erwartungen früh setzen (siehe M07).

**Erfolg messbar machen**
Vor dem Bau festlegen, woran man erkennt, dass ein Agent hilft (z. B. Zeitersparnis pro Plan,
weniger Übertragungsfehler bei m²-Angaben).

**Datenqualität vorab einschätzen**
Ein Extraktions-Agent ist nur so gut wie die Planqualität. Schlecht lesbare Scans, handschriftliche
Vermaßung oder uneinheitliche Layouts verschlechtern die Ergebnisse deutlich.

---

## Agent-Design (Copilot Studio)

**Instruktionen klar und konkret formulieren**
Rolle, Sprache und gewünschtes Ausgabeformat explizit benennen (z. B. "Gib eine Tabelle mit
Raum/Bauteil, Fläche, Einheit zurück") — siehe Prompt-Techniken in M02.

**Ein Tool, eine klare Aufgabe**
Jedes Tool/Skill sollte eine eindeutige, klar beschriebene Fähigkeit abbilden, damit der Agent
zuverlässig erkennt, wann er es einsetzen soll.

**Ergebnisse immer stichprobenartig prüfen**
Insbesondere bei der Anbindung an Solarcomputer: Ergebnisse vor jeder automatisierten
Weiterverarbeitung prüfen, bis genug Erfahrungswerte vorliegen.

**Schrittweise ausbauen**
Erst einen Agenten mit einem Tool zum Laufen bringen (M06), dann erweitern (M07/M08) — nicht alles
auf einmal bauen.

---

## Power Automate

**Trennung Verstehen/Handeln beibehalten**
Copilot Studio versteht (liest den Plan, formuliert die Ausgabe), Power Automate handelt (schreibt
die Werte weiter). Diese Trennung hält die Lösung wartbar.

**Zwischenschritt einplanen, wenn kein direkter Connector existiert**
Für Solarcomputer ist aktuell kein Cloud-Connector bestätigt — Excel/SharePoint als Zwischenschritt
oder Power Automate Desktop als Fallback einplanen (siehe M08).

**Flow-Verlauf als erste Anlaufstelle bei Fehlern**
Der Ausführungsverlauf in Power Automate zeigt genau, an welchem Schritt ein Flow fehlgeschlagen ist.
