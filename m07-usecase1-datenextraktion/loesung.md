# M07 Lösung: Extraktions-Agent für Pläne

## Erwartetes Ergebnis

Eine Tabelle mit den 5 Räumen und den auf dem Plan beschrifteten Flächen:

| Raum             | Fläche  |
| ---------------- | ------- |
| Büro 101         | 20,0 m² |
| Büro 102         | 17,5 m² |
| Flur             | 20,0 m² |
| Besprechungsraum | 30,0 m² |
| Teeküche         | 9,0 m²  |

Bei der DXF-Variante sollte das Ergebnis tendenziell zuverlässiger/vollständiger ausfallen als bei der
PDF-Variante, da die Daten strukturiert vorliegen (LINE-/TEXT-Entitäten statt reinem Rastertext).

## Diskussion im Anschluss

Wo weicht das Ergebnis vom Plan ab, und woran könnte das liegen (Texterkennung, Layout, unklare
Beschriftung)?

## Artefakte

- Getesteter Agent mit Extraktions-Tool
- Extraktions-Tabelle (PDF-Lauf und DXF-Lauf)
