# M08 Theorie: Automatisierung mit Power Automate

> Lesetext für die Teilnehmenden und Showcase-Vorlage für den Trainer. Trainer-Hinweise stehen
> gesammelt im Abschnitt "Trainer-Showcase".

## Lernziel

Nach diesem Modul habt ihr einen Power-Automate-Flow gebaut, der die Agent-Ausgabe entgegennimmt, und
kennt die Optionen zur Anbindung an Solarcomputer.

## Dauer

Tag 2 · 13:15–14:45 · 90 Minuten

## Power-Automate-Flow: Übergabe der Agent-Ausgabe

1. Flow anlegen mit Trigger "wird von Copilot Studio aufgerufen"
2. Eingabe (die strukturierte Tabelle aus M07) als Parameter entgegennehmen
3. Aktion: Werte in eine Excel-/SharePoint-Liste schreiben (als Zwischenschritt/Nachweis)
4. Test: Agent aus M07 aufrufen → prüfen, ob die Werte im Flow ankommen

→ Übung siehe [uebung.md](uebung.md).

## Anbindung Richtung Solarcomputer

Aktuell ist nicht bestätigt, ob es einen direkten Cloud-Connector für Solarcomputer gibt (siehe
[00-eckdaten.md](../00-eckdaten.md)) — das wird vor Ort final mit dem Kunden geklärt. Falls **nein**:
Zwischenschritt über Excel/SharePoint. Falls Solarcomputer eine Import-Schnittstelle (z. B. CSV-Import)
hat: der Flow wird entsprechend erweitert.

## Kurzeinblick Power Automate Desktop

Falls kein Connector/Import existiert, kann Power Automate Desktop Werte automatisiert in die
Solarcomputer-Oberfläche eintragen (Mausklick-/Tastatur-Simulation).

## Trainer-Showcase

- **Power-Automate-Flow (40 Min, Live + Nachbauen):** die 4 Schritte oben live vorführen, TN bauen in
  der Übung mit.
- **Anbindung Richtung Solarcomputer (20 Min):** offene Frage an die Gruppe stellen, gemeinsam Optionen
  durchgehen.
- **Kurzeinblick Power Automate Desktop (15 Min):** kurze Live-Demo mit einer einfachen
  Desktop-Anwendung als Ersatzbeispiel, falls kein Testzugang zu Solarcomputer vorliegt.
- **Quiz-Impuls (Modulende):** einen Freiwilligen den Ablauf des gebauten Flows in eigenen Worten
  erklären lassen (Test-Effekt).

## Leitfragen

Beantwortet die Fragen zuerst selbst, bevor ihr sie aufklappt.

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
