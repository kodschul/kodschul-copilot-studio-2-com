# M09 Lösung: Konzept-Skizze Aufmaßprüfungs-Agent

## Erwartetes Ergebnis

Manueller Soll/Ist-Vergleich der Musterdaten:

| Raum | Soll (CSV) | Ist (Plan) | Befund |
| --- | --- | --- | --- |
| Büro 101 | 20,0 m² | 20,0 m² | passt |
| Büro 102 | 18,0 m² | 17,5 m² | kleine Abweichung |
| Flur | 20,0 m² | 20,0 m² | passt |
| Besprechungsraum | 28,5 m² | 30,0 m² | größere Abweichung |
| Teeküche | 9,0 m² | 9,0 m² | passt |
| Lager | 6,0 m² | — | im Plan nicht enthalten (fehlender Raum) |

Die drei Fälle (passt / Abweichung / fehlender Raum) sind bewusst in den Musterdaten enthalten, um im
Konzept alle drei Fallgruppen zu berücksichtigen.

## Erwartetes Konzept

- **Input:** Massenaufstellung (CSV/Excel) + Plan (PDF/DXF)
- **Tool 1:** Extraktions-Tool aus M07 (Plan → Tabelle mit Fläche je Raum)
- **Vergleichslogik:** Zeilenweiser Abgleich Soll vs. Ist, Toleranzschwelle für "kleine Abweichung"
  definieren (z. B. ±1 m²)
- **Ausgabe:** Tabelle mit Ampel-Markierung (grün = passt, gelb = kleine Abweichung, rot = größere
  Abweichung/fehlender Raum)

## Artefakte

- Manuelle Vergleichstabelle
- Konzept-Skizze (kein fertiger Agent)
