# M07 Übung: Extraktions-Agent für Pläne

## Zeit

Eingebettet in Modul 7 (Live + Nachbauen), einzeln oder zu zweit

## Ziel

Den in M06 gebauten Agenten (oder einen neuen) um ein Extraktions-Tool erweitern, das aus einem Plan
Flächen-/Mengendaten als Tabelle ausgibt.

## Material

- Copilot-Studio-Zugang
- Musterdaten: [../musterdaten/beispiel-plan.pdf](../musterdaten/beispiel-plan.pdf), [../musterdaten/beispiel-plan.dxf](../musterdaten/beispiel-plan.dxf)

## Vorgehen

1. Agenten um ein Tool "Dokument/Plan einlesen" erweitern.
2. Instruktionen ergänzen: "Extrahiere alle Flächen-/Mengenangaben aus dem Plan und gib sie als
   Tabelle mit Spalten Raum/Bauteil, Fläche, Einheit zurück."
3. Mit [../musterdaten/beispiel-plan.pdf](../musterdaten/beispiel-plan.pdf) testen (5 Räume: Büro 101,
   Büro 102, Flur, Besprechungsraum, Teeküche).
4. Mit [../musterdaten/beispiel-plan.dxf](../musterdaten/beispiel-plan.dxf) (gleicher Grundriss,
   strukturiertes Format) testen und Ergebnisse vergleichen.

## Abnahme

- Agent liefert für beide Dateiformate eine Tabelle mit Raum/Bauteil, Fläche, Einheit.
- Abweichungen zwischen erwartetem und tatsächlichem Ergebnis wurden diskutiert.
