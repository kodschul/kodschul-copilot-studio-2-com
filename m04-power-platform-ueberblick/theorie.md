# M04 Theorie: Power Platform im Überblick

## Lernziel

Grundbausteine von Power Automate (Trigger, Aktion, Connector) kennen, wissen wann Power Automate
Desktop statt Cloud sinnvoll ist, Lizenzrahmen von M365 Business kennen.

## Dauer

Tag 1 · 15:00–16:15 · 75 Minuten

## Power Automate (Cloud): Grundbausteine (25 Min, Live-Screenshare)

- **Trigger** (was löst den Flow aus, z. B. "neue Datei in SharePoint" oder "von Copilot Studio aufgerufen")
- **Aktion** (was passiert dann, z. B. "Zeile in Excel hinzufügen", "E-Mail senden")
- **Connector** (die Verbindung zu einem System, z. B. SharePoint-, Excel-, Outlook-Connector)
- Einfaches Beispiel gemeinsam bauen: Trigger "manuell" → Aktion "Excel-Zeile hinzufügen"

## Power Automate Desktop: Abgrenzung (15 Min)

Für Alt-/Desktop-Anwendungen ohne moderne Schnittstelle (Cloud-Connector) gedacht — simuliert
Mausklicks/Tastatureingaben. Relevant für EFG, falls Solarcomputer keinen direkten Cloud-Connector hat
(ausführlicher in M08).

## Lizenzrahmen M365 Business (10 Min)

Mit M365 Business ist die Basisnutzung von Power Automate und Copilot Studio bereits möglich (siehe
[00-eckdaten.md](../00-eckdaten.md)). Grenzen ansprechen: Premium-Connectors oder hohe Nutzungsvolumen
können Zusatzkosten auslösen.

## Wie erweitert man die Plattform selbstständig (15 Min)

Connector-Bibliothek durchsuchen (hunderte vorgefertigte Connectors). Kurzer Hinweis auf Custom
Connectors (falls kein Standard-Connector für Solarcomputer existiert) — als Ausblick.

→ Übung siehe [uebung.md](uebung.md).

## Leitfragen

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
