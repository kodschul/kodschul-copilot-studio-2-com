# M08 Lösung: Power-Automate-Flow zur Datenübergabe

## Erwartetes Ergebnis

Ein Flow mit:
- Trigger: "Wenn ein Flow von einem Copilot Agent aufgerufen wird", mit Parametern passend zur Tabelle
  aus M07 (Raum/Bauteil, Fläche, Einheit)
- Aktion: "Zeile in Tabelle hinzufügen" (Excel Online) oder "Element erstellen" (SharePoint)

Nach End-to-End-Test (Agent aus M07 aufrufen) erscheinen die extrahierten Werte automatisch als neue
Zeile(n) in der Excel-Tabelle/SharePoint-Liste.

## Empfehlung für die Solarcomputer-Anbindung (Diskussionsergebnis)

Da aktuell kein Connector bestätigt ist: Excel/SharePoint als Zwischenschritt nutzen, bis mit
IT/Microsoft-Partner geklärt ist, ob ein direkter Connector oder Import existiert. Andernfalls Power
Automate Desktop zur automatisierten Eingabe in die Solarcomputer-Oberfläche.

## Artefakte

- Funktionsfähiger, end-to-end getesteter Flow
