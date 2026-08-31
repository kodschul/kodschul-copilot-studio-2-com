# M03 Theorie: Copilot Studio im Überblick

## Lernziel

Aufbau eines Copilot-Studio-Agenten (Instruktionen, Wissen, Tools, Themen, Testfenster) kennen und das
Zusammenspiel Copilot Studio ↔ Power Automate ↔ M365 verstehen.

## Dauer

Tag 1 · 13:15–14:45 · 90 Minuten

## Aufbau der Oberfläche (20 Min, Live-Screenshare)

- Startseite/Agenten-Übersicht → neuen Agenten anlegen
- Kernbereiche: Übersicht/Beschreibung, **Instruktionen** (System-Prompt), **Wissen** (Knowledge),
  **Tools/Skills**, **Themen** (kurz erwähnen, Fokus liegt auf Tools/Skills), **Testfenster**
- Testfenster direkt im Editor nutzen, um Änderungen sofort auszuprobieren

## Skills & Tools: Konzept, Unterschied, wann was verwenden (20 Min)

Vordefinierte Konnektoren-Tools (z. B. SharePoint durchsuchen) vs. selbst angelegte Tools, die einen
Power-Automate-Flow auslösen. Eigenes Tool bauen, sobald ein individueller Prozess (wie die
Solarcomputer-Anbindung) nötig ist. Ein Tool braucht eine klare Beschreibung, damit der Agent versteht,
*wann* er es einsetzen soll (Bezug zu Prompt-Techniken aus M02).

## Knowledge/Wissensquellen anbinden (15 Min)

Dateien, SharePoint-Seiten oder Webseiten als Wissensbasis hinzufügen, auf die der Agent antworten
kann, ohne zu halluzinieren.

## Konnektoren-Prinzip — Brücke zu Power Automate (15 Min)

Ein Tool in Copilot Studio kann direkt einen Power-Automate-Flow als "Backend" nutzen. Copilot Studio =
Gesprächsebene/Verstehen, Power Automate = Ausführungsebene/Handeln.

## Einsatzszenarien für Ingenieurbüros & Zusammenspiel mit M365 (20 Min)

Beispiele: Angebotsanfragen vorstrukturieren, Plan-Daten extrahieren, Status-Updates aus
Teams/SharePoint zusammenfassen. Zusammenspiel Copilot Studio ↔ Power Automate ↔ M365 (SharePoint als
Ablage für Pläne).

→ Übung siehe [uebung.md](uebung.md).

## Leitfragen

<details>
<summary>Aus welchen Kernbereichen besteht ein Copilot-Studio-Agent?</summary>

Instruktionen, Wissen, Tools/Skills, Themen und Testfenster.

</details>

<details>
<summary>Was ist der Unterschied zwischen einem vordefinierten Konnektor-Tool und einem selbstgebauten Tool?</summary>

Vordefiniert = Standardfall (z. B. SharePoint-Suche). Selbstgebaut = individueller Prozess über einen
eigenen Power-Automate-Flow (z. B. Solarcomputer-Anbindung).

</details>

<details>
<summary>Wozu dient "Knowledge" in Copilot Studio?</summary>

Wissensquellen anbinden, damit der Agent auf Basis echter Daten statt Vermutungen antwortet.

</details>

<details>
<summary>Welche Ebene "versteht", welche Ebene "handelt"?</summary>

Copilot Studio versteht, Power Automate handelt.

</details>
