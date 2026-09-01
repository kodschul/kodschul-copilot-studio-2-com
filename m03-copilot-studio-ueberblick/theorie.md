# M03 Theorie: Copilot Studio im Überblick

> Lesetext für die Teilnehmenden und Showcase-Vorlage für den Trainer. Trainer-Hinweise stehen
> gesammelt im Abschnitt "Trainer-Showcase".

## Lernziel

Nach diesem Modul kennt ihr den Aufbau eines Copilot-Studio-Agenten (Instruktionen, Wissen, Tools,
Themen, Testfenster) und versteht das Zusammenspiel Copilot Studio ↔ Power Automate ↔ M365.

## Dauer

Tag 1 · 13:15–14:45 · 90 Minuten

## Aufbau der Oberfläche

Ein Agent in Copilot Studio besteht aus folgenden Kernbereichen: Übersicht/Beschreibung,
**Instruktionen** (System-Prompt), **Wissen** (Knowledge), **Tools/Skills**, **Themen** (klassische,
ältere Konversationsabläufe — in dieser Schulung nicht im Fokus) und ein **Testfenster**, in dem man
Änderungen direkt ausprobieren kann.

## Skills & Tools: Konzept, Unterschied, wann was verwenden

Es gibt vordefinierte Konnektoren-Tools (z. B. SharePoint durchsuchen, E-Mail senden) und selbst
angelegte Tools, die einen Power-Automate-Flow auslösen. Ein eigenes Tool baut man, sobald ein
individueller Prozess (wie die Solarcomputer-Anbindung) nötig ist, den es standardmäßig nicht gibt.
Wichtig: ein Tool braucht eine klare Beschreibung, damit der Agent versteht, _wann_ er es einsetzen
soll (Bezug zu den Prompt-Techniken aus M02).

## Knowledge/Wissensquellen anbinden

Dateien, SharePoint-Seiten oder Webseiten können als Wissensbasis hinzugefügt werden, auf die der
Agent antworten kann, ohne zu halluzinieren.

## Konnektoren-Prinzip — Brücke zu Power Automate

Ein Tool in Copilot Studio kann direkt einen Power-Automate-Flow als "Backend" nutzen. Copilot Studio =
Gesprächsebene/Verstehen, Power Automate = Ausführungsebene/Handeln — diese Trennung ist zentral für das
Verständnis der Architektur.

## Einsatzszenarien für Ingenieurbüros & Zusammenspiel mit M365

Beispiele: Angebotsanfragen vorstrukturieren, Plan-Daten extrahieren, Status-Updates aus
Teams/SharePoint zusammenfassen, Planner-Aufgaben automatisch anlegen. Zusammenspiel Copilot Studio ↔
Power Automate ↔ M365 (SharePoint als Ablage für Pläne, Planner für Aufgaben aus dem Aufmaß-Use-Case).

→ Übung siehe [uebung.md](uebung.md).

## Trainer-Showcase

- **Aufbau der Oberfläche (20 Min, Live-Screenshare):** Startseite/Agenten-Übersicht → neuen Agenten
  anlegen, alle Kernbereiche einmal live anklicken.
- **Skills & Tools (20 Min):** Beispiel für ein vordefiniertes und ein selbstgebautes Tool live
  gegenüberstellen.
- **Knowledge (15 Min):** eine Wissensquelle live hinzufügen.
- **Konnektoren-Prinzip (15 Min):** die Trennung Verstehen/Handeln anhand eines einfachen Beispiels
  zeigen.
- **Einsatzszenarien & M365-Zusammenspiel (20 Min):** Beispiele im Plenum diskutieren.
- **Prequestion (zu Beginn):** "Welche eurer M365-Tools glaubt ihr, lassen sich direkt mit Copilot
  Studio verbinden?"

## Leitfragen

Beantwortet die Fragen zuerst selbst, bevor ihr sie aufklappt.

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
