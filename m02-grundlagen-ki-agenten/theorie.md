# M02 Theorie: Grundlagen KI-Agenten

> Lesetext für die Teilnehmenden und Showcase-Vorlage für den Trainer. Trainer-Hinweise stehen
> gesammelt im Abschnitt "Trainer-Showcase".

## Lernziel

Nach diesem Modul könnt ihr Agent, Skill/Tool und Prompt definieren und voneinander abgrenzen,
Prompt-Techniken anwenden und die Grenzen von KI-Agenten einschätzen.

## Dauer

Tag 1 · 10:45–12:15 · 90 Minuten

## Was ist ein Agent?

Ein Agent ist ein KI-System, das (1) eine Aufgabe versteht, (2) selbst entscheidet, welche
Schritte/Werkzeuge nötig sind, und (3) diese Schritte ausführt — nicht nur antwortet, sondern **handelt**.

Abgrenzung zum Chatbot: ein klassischer Chatbot antwortet nur auf Basis von Text; ein Agent kann
Werkzeuge (Skills/Tools) aufrufen, Daten aus Dokumenten ziehen oder Systeme ansteuern.

Abgrenzung zur klassischen Automatisierung (Power Automate ohne KI): diese folgt festen Regeln
("wenn X, dann Y"); ein Agent kann auch mit unstrukturierten Eingaben (z. B. einem PDF-Plan) umgehen.

## Was ist ein Skill / ein Tool?

Ein **Skill/Tool** ist eine konkrete Fähigkeit, die der Agent aufrufen kann — z. B. "Datei lesen",
"Suche in SharePoint", "Flow in Power Automate auslösen". Der Agent entscheidet selbst, _wann_ er
welches Tool braucht. Beispiel für EFG: ein Tool "PDF-Plan einlesen" + ein Tool "Werte an Power
Automate übergeben" ergeben zusammen den Datenextraktions-Agenten aus M07/M08.

## Was ist ein Prompt?

Die Anweisung/Eingabe an den Agenten. Es gibt zwei Ebenen: **Nutzer-Prompt** (was ihr eingebt) vs.
**System-Prompt/Instruktionen** (fest im Agenten hinterlegt, z. B. "Antworte immer auf Deutsch,
extrahiere Flächenangaben als Tabelle").

## Prompt-Techniken

- **Kontext geben:** relevante Informationen mitliefern.
- **Rolle zuweisen:** "Du bist ein Assistent für Gebäudetechnik-Aufmaße".
- **Beispiele geben (Few-Shot):** gewünschtes Ausgabeformat zeigen.
- **Schritt-für-Schritt anweisen:** komplexe Aufgaben in Teilschritte zerlegen.

→ Übung siehe [uebung.md](uebung.md).

## Grenzen & realistische Erwartungen

- Halluzination: der Agent kann plausibel klingende, aber falsche Werte liefern.
- Datenqualität entscheidet: schlechte Scans, handschriftliche Vermaßung, uneinheitliche Pläne.
- Kein "Autopilot": Ergebnisse müssen anfangs stichprobenartig geprüft werden.

## Trainer-Showcase

- **Was ist ein Agent? (15 Min):** Definition und beide Abgrenzungen (Chatbot, klassische
  Automatisierung) im Plenum erläutern.
- **Was ist ein Skill/Tool? (15 Min):** Beispiel "PDF-Plan einlesen" + "Werte übergeben" als
  Vorgeschmack auf M07/M08 nennen.
- **Was ist ein Prompt? (10 Min):** Nutzer-Prompt vs. Instruktionen gegenüberstellen.
- **Prompt-Techniken (15 Min, praxisnah):** die vier Techniken kurz vorführen, danach in die Übung
  überleiten.
- **Grenzen & realistische Erwartungen (10 Min):** offen ansprechen, insbesondere im Hinblick auf
  Solarcomputer-Weitergabe in M07/M08.
- **Live-Demo (15 Min):** fertigen Agenten zeigen, der aus einem Beispiel-Plan Flächendaten extrahiert
  und tabellarisch ausgibt (Vorgeschmack auf M07/M08). Bewusst als Blackbox zeigen — "so wird es am
  Ende aussehen, morgen baut ihr das selbst".
- **Prequestion (vor "Was ist ein Agent?"):** "Was denkt ihr, kann ein Agent, was ein normaler Chatbot
  nicht kann?"

## Leitfragen

Beantwortet die Fragen zuerst selbst, bevor ihr sie aufklappt.

<details>
<summary>Was unterscheidet einen Agenten von einem Chatbot?</summary>

Ein Agent kann Werkzeuge/Tools aufrufen und damit handeln, nicht nur antworten.

</details>

<details>
<summary>Was ist ein Skill/Tool in Copilot Studio?</summary>

Eine konkrete Fähigkeit, die der Agent bei Bedarf aufruft (z. B. Datei lesen, Flow auslösen).

</details>

<details>
<summary>Nennt eine Prompt-Technik.</summary>

Kontext geben, Rolle zuweisen, Beispiele geben oder Schritt-für-Schritt anweisen.

</details>

<details>
<summary>Warum sollte man Agenten-Ergebnisse anfangs immer prüfen?</summary>

Wegen Halluzinationsgefahr und schwankender Datenqualität — besonders wichtig, bevor Ergebnisse
automatisiert weiterverarbeitet werden (z. B. Richtung Solarcomputer).

</details>
