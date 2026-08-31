# M08 Übung: Power-Automate-Flow zur Datenübergabe

## Zeit

Eingebettet in Modul 8 (Live + Nachbauen), einzeln oder zu zweit

## Ziel

Einen Power-Automate-Flow bauen, der die strukturierte Tabelle aus dem Extraktions-Agenten (M07)
entgegennimmt und in Excel/SharePoint schreibt.

## Material

- Power-Automate-Zugang
- Der Agent aus M07

## Vorgehen

1. Neuen Flow anlegen mit Trigger "Wenn ein Flow von einem Copilot Agent aufgerufen wird".
2. Eingabeparameter definieren, die zur Tabellenstruktur aus M07 passen (Raum/Bauteil, Fläche, Einheit).
3. Aktion ergänzen: Zeile(n) in eine Excel-Tabelle oder SharePoint-Liste schreiben.
4. Flow speichern, den Agenten aus M07 damit verbinden (als Tool hinzufügen) und end-to-end testen.

## Abnahme

- Nach Aufruf des Agenten mit dem Beispiel-Plan erscheinen die extrahierten Werte automatisch in der
  Excel-Tabelle/SharePoint-Liste.
- Der nächste Schritt Richtung Solarcomputer (Connector, Zwischenschritt, Power Automate Desktop) wurde
  kurz besprochen.
