# M08 Theorie: Automatisierung mit Power Automate

## Lernziel

Einen Power-Automate-Flow bauen, der die Agent-Ausgabe entgegennimmt; Optionen zur Anbindung an
Solarcomputer kennen.

## Dauer

Tag 2 · 13:15–14:45 · 90 Minuten

## Power-Automate-Flow: Übergabe der Agent-Ausgabe (40 Min, Live + Nachbauen)

1. Flow anlegen mit Trigger "wird von Copilot Studio aufgerufen"
2. Eingabe (die strukturierte Tabelle aus M07) als Parameter entgegennehmen
3. Aktion: Werte in eine Excel-/SharePoint-Liste schreiben (als Zwischenschritt/Nachweis)
4. Test: Agent aus M07 aufrufen → prüfen, ob die Werte im Flow ankommen

→ Übung siehe [uebung.md](uebung.md).

## Anbindung Richtung Solarcomputer (20 Min) — vor Ort mit Kunde final klären

- Frage an die Gruppe: gibt es einen direkten Cloud-Connector für Solarcomputer? (bisher nicht
  bekannt, siehe [00-eckdaten.md](../00-eckdaten.md))
- Falls **nein**: Zwischenschritt über Excel/SharePoint zeigen
- Falls Solarcomputer eine Import-Schnittstelle (z. B. CSV-Import) hat: Flow entsprechend erweitern

## Kurzeinblick Power Automate Desktop (15 Min)

Falls kein Connector/Import existiert: Power Automate Desktop kann Werte automatisiert in die
Solarcomputer-Oberfläche eintragen. Kurze Live-Demo mit einer einfachen Desktop-Anwendung als
Ersatzbeispiel, falls kein Testzugang zu Solarcomputer vorliegt.

## Leitfragen

<details>
<summary>Erklärt den Ablauf des gebauten Flows in eigenen Worten.</summary>

Trigger (Agent ruft den Flow auf) → Eingabe (strukturierte Tabelle) → Aktion (Werte in Excel/SharePoint
schreiben) → Ergebnis (Werte sind im Zielsystem sichtbar).

</details>

<details>
<summary>Was tun, wenn kein Solarcomputer-Connector existiert?</summary>

Zwischenschritt über Excel/SharePoint, oder Power Automate Desktop zur automatisierten Eingabe in die
Solarcomputer-Oberfläche.

</details>
