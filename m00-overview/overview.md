# Kursüberblick – KI-Agenten bauen mit Microsoft Copilot & Copilot Studio

## Kursziel und Abschlussbild

Der Kurs zeigt, wie aus einem realistischen Supportbedarf ein geprüfter KI-Agent entsteht: erst als Copilot-Chat-Agent, dann als Copilot-Studio-Agent auf dem GitHub-Copilot-Harness.

Am Ende liegt ein beobachtbares Ergebnis vor: der Nordwind IT-Helfer beantwortet Testfragen, nutzt vorbereitete Quellen, enthält Skills, kann ein Tool oder MCP nutzen, ist für Teams vorbereitet und besitzt Governance-Kurzcheck sowie Aktionsplan.

## Zielgruppe und Voraussetzungen

- Zielgruppe: Maker, Fachbereich, Business-Anwender:innen und technisch interessierte Rollen ohne vorausgesetzte Programmierkenntnisse.
- Einstieg: erste KI-Chat-Erfahrung ist hilfreich, aber keine Voraussetzung.
- Tag 1: Microsoft 365 Copilot oder Copilot Chat mit Agent-Builder-Berechtigung.
- Tag 2: Copilot Studio, GitHub-Copilot-Harness, Credits oder Pay-as-you-go, Sandbox, DLP-Freigaben, SharePoint-Testsite, Teams-Kanal und Publish-Rechte.
- Alle Übungen nutzen fiktive Nordwind-Daten aus dem [Projektmaterial](../project/README.md); reale Unternehmens- oder Personendaten bleiben ausgeschlossen.

## Agenda Tag 1

| Zeit | Inhalt | Labs und Checkpoints |
| --- | --- | --- |
| 09:00–09:10 | Orientierung, Trainerrolle, Kursrahmen | Gemeinsamer Start |
| 09:10–09:40 | Teilnehmerkontext und Erwartungen | Vorstellungsfolie, Erwartungsmuster |
| 09:40–09:50 | Kursziel, roter Faden, Arbeitsweise | The Nextise Agentic Way in drei Sätzen |
| 09:50–10:05 | Modul 1, Thema „Wie KI entstanden ist“ | KI-Zeitleiste und Begriffsgrundlage (nur Input) |
| 10:05–10:30 | Modul 1, Thema „Wie ein Sprachmodell antwortet“ | LLM, Kontext, Grounding (nur Input, Plenumsfragen) |
| 10:30–10:45 | Pause |  |
| 10:45–11:05 | Modul 2, Lab 2.1 | Schlechten und besseren Beispielprompt ausprobieren und vergleichen |
| 11:05–11:30 | Modul 2, Lab 2.2 | Zero-Shot, Few-Shot/CoT und Qualitätsvergleich |
| 11:30–11:55 | Modul 2, Lab 2.3 | Instruktions-Skelett für den IT-Helfer |
| 11:55–12:15 | Modul 2, Lab 2.4 | HITL-Gliederung mit Entscheidungsstellen |
| 12:15–13:15 | Mittagspause |  |
| 13:15–13:45 | Modul 3, Lab 3.1 | Agent, Skill, Tool und Agentic Loop einordnen |
| 13:45–13:55 | Modul 3, Lab 3.2 | Copilot Chat und Agent Builder beobachten |
| 13:55–14:45 | Modul 3, Lab 3.3 | Einfacher Nordwind IT-Helfer plus Testlog |
| 14:45–15:00 | Pause |  |
| 15:00–15:25 | Modul 4, Lab 4.1 | Problem-Solver: Canvas und Top-1-Empfehlung |
| 15:25–15:45 | Modul 4, Lab 4.2 | Solution Architect: Kurzkonzept und Skill-Liste |
| 15:45–16:10 | Modul 4, Lab 4.3 | Skill-Generator: System-Prompt und `SKILL.md` |
| 16:10–16:25 | Modul 4, Lab 4.4 | Direkter Bau vs. Kette vergleichen |
| 16:25–16:30 | Tagesabschluss | Artefakte sichern, Brücke zu Tag 2 |

## Agenda Tag 2

| Zeit | Inhalt | Labs und Checkpoints |
| --- | --- | --- |
| 09:00–09:15 | Recap und Arbeitsfähigkeit | Quiz, Artefakt-Check, Tagesziel |
| 09:15–09:50 | Modul 5, Lab 5.1 | Chat-Agent mit Wissen optimieren, Vorher/Nachher-Test |
| 09:50–10:30 | Modul 5, Lab 5.2 | Entscheidungsmatrix Chat-Agent vs. Studio-Harness |
| 10:30–10:45 | Pause |  |
| 10:45–11:30 | Modul 6, Lab 6.1 | Studio-Agent auf GitHub-Copilot-Harness anlegen |
| 11:30–12:15 | Modul 6, Lab 6.2 | `SKILL.md` und generierten Skill testen |
| 12:15–13:15 | Mittagspause |  |
| 13:15–13:40 | Modul 7, Lab 7.1 | Lesenden Konnektor als Tool auslösen |
| 13:40–14:10 | Modul 7, Lab 7.2 | Schreibgeschützten MCP-Server prüfen |
| 14:10–14:45 | Modul 7, Lab 7.3 | Testset, Evaluation und Verbesserung |
| 14:45–15:00 | Pause |  |
| 15:00–15:25 | Modul 8, Lab 8.1 | Teams-Veröffentlichung oder Publish-Protokoll |
| 15:25–16:05 | Modul 8, Lab 8.2 | Workflow mit Freigabe als Agent-Tool |
| 16:05–16:27 | Modul 8, Lab 8.3 | Governance-Kurzcheck, Showcase, Aktionsplan |
| 16:27–16:30 | Abschluss | Offene Fragen, nächste Schritte |

## Modul- und Projektstruktur

- Modul 1 schafft die gemeinsame Sprache für KI, LLM, Kontext, Grounding und Agenten.
- Modul 2 macht aus Einzelprompts wiederverwendbare Agenten-Instruktionen.
- Modul 3 baut den ersten Nordwind IT-Helfer als Copilot-Chat-Agent ohne Wissensquelle.
- Modul 4 erzeugt mit drei Assistenten Canvas, Kurzkonzept, System-Prompt und `SKILL.md`.
- Modul 5 optimiert den Chat-Agenten mit Nordwind-Wissen und begründet die Harness-Wahl.
- Modul 6 baut denselben Fall in Copilot Studio mit GitHub-Copilot-Harness und Skills nach.
- Modul 7 ergänzt Konnektor, MCP und Evaluation.
- Modul 8 macht den Agenten nutzbar: Teams, Workflow, Governance und persönlicher Aktionsplan.

## Arbeitsmethode und Übungskonventionen

- `-thx.md` enthält Theorie, Begriffe, Beispiele und Fazit.
- `-exc.md` enthält die praktische Aufgabe mit Checkpoints, Abschlusskriterien und Fallback.
- `-sol.md` enthält die passende Musterlösung mit Ergebnis, Begründung und Grenzen.
- Baseline-Aufgaben reichen für den gemeinsamen Pfad; Erweiterungen und Challenges bleiben optional.
- Checkpoints prüfen beobachtbare Artefakte: Antwort, Matrix, Testlog, Skill, Toollauf, Publish-Protokoll oder Aktionsplan.

## Umgebung und Sicherheit

- Nur Sandbox, Dev-Umgebung, Testsite und fiktive Nordwind-Daten verwenden.
- Keine produktiven Daten, echten Personeninformationen, geheimen URLs oder Zugangsdaten in Prompts, Quellen, Tools oder Workflows einfügen.
- Schreibende Aktionen brauchen menschliche Freigabe und klare Rückrollbarkeit.
- DLP, Konnektoren, MCP, Credits, Publish-Rechte und UI-Pfade sind vor Durchführung tenantabhängig zu prüfen.
- Falls Tag-2-Zugriff fehlt, bleibt das Lernziel über Demo, Screenshots, Protokolle und Chat-Agent-Weiterarbeit erreichbar.

## Vorstellungsfolie für Teilnehmer:innen

- Name und aktuelle Rolle
- Beruflicher Hintergrund und aktuelle Tätigkeit
- Weg in das aktuelle Arbeitsfeld
- Organisation und Zugehörigkeitsdauer
- Optional: Stadt oder Region und lokales Wetter
- Bisherige Erfahrung mit KI, Copilot, Agenten oder Automatisierung
- Erwartungen an den Kurs
- Geplanter eigener Anwendungsfall oder Arbeitsauftrag
- Persönliche Angaben sind freiwillig; einzelne Punkte können ausgelassen werden.

## Weitere Überblicksdateien

- [Themenliste](topics.md)
- [Glossar](glossary.md)
- [Best Practices](best-practices.md)
- [FAQ](faq.md)
