# M04 Theorie: Power Platform im Überblick

> Lesetext für die Teilnehmenden und Showcase-Vorlage für den Trainer. Trainer-Hinweise stehen
> gesammelt im Abschnitt "Trainer-Showcase".

## Lernziel

Nach diesem Modul kennt ihr die Grundbausteine von Power Automate (Trigger, Aktion, Connector), wisst
wann Power Automate Desktop statt Cloud sinnvoll ist, und kennt den Lizenzrahmen von M365 Business.

## Dauer

Tag 1 · 15:00–16:15 · 75 Minuten

## Power Automate (Cloud): Grundbausteine

- **Trigger** (was löst den Flow aus, z. B. "neue Datei in SharePoint" oder "von Copilot Studio aufgerufen")
- **Aktion** (was passiert dann, z. B. "Zeile in Excel hinzufügen", "E-Mail senden")
- **Connector** (die Verbindung zu einem System, z. B. SharePoint-, Excel-, Outlook-Connector)

## Power Automate Desktop: Abgrenzung

Power Automate Desktop ist für Alt-/Desktop-Anwendungen ohne moderne Schnittstelle (Cloud-Connector)
gedacht — es simuliert Mausklicks/Tastatureingaben. Relevant für EFG, falls Solarcomputer keinen
direkten Cloud-Connector hat und Daten stattdessen über die Desktop-Oberfläche eingetragen werden
müssen (ausführlicher in M08).

## Lizenzrahmen M365 Business

Mit M365 Business ist die Basisnutzung von Power Automate und Copilot Studio bereits möglich (siehe
[00-eckdaten.md](../00-eckdaten.md)). Bestimmte Premium-Connectors oder hohe Nutzungsvolumen können
Zusatzkosten auslösen — im Zweifel vor Ort/mit Microsoft-Partner klären.

## Wie erweitert man die Plattform selbstständig

Die Connector-Bibliothek umfasst hunderte vorgefertigte Connectors. Falls kein Standard-Connector für
eine Software wie Solarcomputer existiert, gibt es außerdem die Möglichkeit, einen Custom Connector
anzulegen — das ist in dieser Schulung ein Ausblick, kein Tiefeninhalt.

→ Übung siehe [uebung.md](uebung.md).

## Trainer-Showcase

- **Power Automate Grundbausteine (25 Min, Live-Screenshare):** ein einfaches Beispiel gemeinsam bauen
  — Trigger "manuell" → Aktion "Excel-Zeile hinzufügen".
- **Power Automate Desktop (15 Min):** kurze Live-Demo, falls Zeit reicht, sonst nur Konzept erklären.
- **Lizenzrahmen (10 Min):** Grenzen ansprechen (Premium-Connectors, Nutzungsvolumen).
- **Plattform erweitern (15 Min):** Connector-Bibliothek kurz live zeigen, Custom Connectors als
  Ausblick erwähnen.
- **Prequestion (zu Beginn):** "Was glaubt ihr, ist der Unterschied zwischen Power Automate Cloud und
  Power Automate Desktop?"

## Leitfragen

Beantwortet die Fragen zuerst selbst, bevor ihr sie aufklappt.

<details>
<summary>Was ist ein Trigger?</summary>

Das Ereignis, das einen Flow startet.

</details>

<details>
<summary>Was ist ein Connector?</summary>

Die Verbindung zwischen Power Automate und einem System/einer App.

</details>

<details>
<summary>Wann braucht man Power Automate Desktop statt Cloud?</summary>

Wenn kein Cloud-Connector existiert, z. B. bei älteren Desktop-Programmen.

</details>

<details>
<summary>Was ist in M365 Business bereits enthalten?</summary>

Die Basisnutzung von Power Automate und Copilot Studio.

</details>
