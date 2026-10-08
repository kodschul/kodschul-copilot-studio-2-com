# Best Practices

Übergreifende Praktiken aus allen Modulen. Jede Praxis nennt Grund und Entscheidungskriterium.

## Begriffe und Entscheidungen

### 1. Begriffe vor Toolschritten klären
- Praxis: Begriffe vor Toolschritten klären.
- Grund: Ein gemeinsames Vokabular verhindert, dass Prompt, Chat, Agent, Skill und Tool vermischt werden.
- Kriterium: Eine Entscheidung ist tragfähig, wenn sie den Begriff korrekt und mit Lab-Bezug nutzt.

### 2. Kleinsten passenden Bauweg wählen
- Praxis: Kleinsten passenden Bauweg wählen.
- Grund: Ein mächtiger Harness erhöht Setup, Kosten, Latenz und Governance-Aufwand.
- Kriterium: Chat-Agent reicht bei Wissens-FAQ; GitHub-Copilot-Harness lohnt bei mehrstufigen Zielen.

### 3. GitHub-Copilot-Harness korrekt einordnen
- Praxis: GitHub-Copilot-Harness korrekt einordnen.
- Grund: Der Begriff bezeichnet ein Copilot-Studio-Harness, nicht den GitHub-Copilot-Dienst.
- Kriterium: Jede Empfehlung nennt diese Abgrenzung ausdrücklich.

### 4. Nicht-Wechselbarkeit früh prüfen
- Praxis: Nicht-Wechselbarkeit früh prüfen.
- Grund: Der Harness wird beim Erstellen gewählt und ist später nicht einfach übertragbar.
- Kriterium: Vor dem Bau liegt eine begründete Matrix vor.

### 5. Standard-Harness nur als Vergleich nutzen
- Praxis: Standard-Harness nur als Vergleich nutzen.
- Grund: Der Kurs fokussiert Chat-Agent und GitHub-Copilot-Harness.
- Kriterium: Feste Topics werden eingeordnet, aber nicht zum Hauptpfad gemacht.

## Prompting und Instruktionen

### 6. Rolle, Kontext, Aufgabe und Format trennen
- Praxis: Rolle, Kontext, Aufgabe und Format trennen.
- Grund: Fehlende Bausteine erzeugen plausible, aber unpassende Antworten.
- Kriterium: Promptqualität steigt sichtbar im Vorher/Nachher-Vergleich.

### 7. Änderbare Fakten aus Instruktionen heraushalten
- Praxis: Änderbare Fakten aus Instruktionen heraushalten.
- Grund: Richtlinien und Listen ändern sich häufiger als Verhaltensregeln.
- Kriterium: Fakten stehen in Knowledge, nicht im System-Prompt.

### 8. Verbote konkret formulieren
- Praxis: Verbote konkret formulieren.
- Grund: Unklare Verbote erzeugen zu breite oder zu harte Ablehnung.
- Kriterium: Grenzen nennen betroffene Fälle und erwünschte Ersatzhandlung.

### 9. Few-Shot gezielt einsetzen
- Praxis: Few-Shot gezielt einsetzen.
- Grund: Beispiele helfen bei Format und Qualitätsstandard, verlängern aber Kontext.
- Kriterium: Few-Shot wird nur genutzt, wenn Formattreue wichtiger als Kürze ist.

### 10. Chain-of-Thought nicht zur Pflicht machen
- Praxis: Chain-of-Thought nicht zur Pflicht machen.
- Grund: Schrittweise Begründung ist für riskante Entscheidungen nützlich, aber oft zu ausführlich.
- Kriterium: Antworten bleiben prüfbar, ohne interne Denkspuren zu erzwingen.

## Human-in-the-loop und Methodik

### 11. Problem vor Lösung klären
- Praxis: Problem vor Lösung klären.
- Grund: Zu frühe Lösungswahl konserviert falsche Annahmen.
- Kriterium: Canvas und Top-1-Empfehlung existieren vor Architektur und Skill.

### 12. Zwischenergebnisse aktiv prüfen
- Praxis: Zwischenergebnisse aktiv prüfen.
- Grund: KI-generierte Artefakte wirken konsistent, können aber falsche Annahmen enthalten.
- Kriterium: Jede Kettenstufe hat einen Checkpoint.

### 13. Menschliche Freigaben vor Nebenwirkungen platzieren
- Praxis: Menschliche Freigaben vor Nebenwirkungen platzieren.
- Grund: Nachträgliche Kontrolle verhindert keine falsche Schreibaktion.
- Kriterium: Freigabe liegt vor Ticketanlage, Nachricht oder anderer Wirkung.

### 14. Kette nicht als Autopilot verstehen
- Praxis: Kette nicht als Autopilot verstehen.
- Grund: The Nextise Agentic Way nutzt KI als Strukturhilfe, nicht als Verantwortungsersatz.
- Kriterium: Entscheidungen bleiben dokumentiert und menschlich bestätigt.

### 15. Vergleich Direktbau vs. Kette sichern
- Praxis: Vergleich Direktbau vs. Kette sichern.
- Grund: Der Nutzen der Methodik wird erst im Unterschied sichtbar.
- Kriterium: Lab 4.4 nennt mindestens zwei Qualitätsunterschiede.

## Chat-Agent und Wissen

### 16. Erst absichtlich ohne Wissen testen
- Praxis: Erst absichtlich ohne Wissen testen.
- Grund: Fehlendes Grounding wird sichtbar, bevor Quellen angebunden werden.
- Kriterium: Das Testlog enthält Schwächen des einfachen Agenten.

### 17. Quellenbezug gegen Dateifakten prüfen
- Praxis: Quellenbezug gegen Dateifakten prüfen.
- Grund: Klingende Antworten sind kein Nachweis für Grounding.
- Kriterium: Eine Antwort wird mit einem Nordwind-Fakt abgeglichen.

### 18. Wissen klein und relevant halten
- Praxis: Wissen klein und relevant halten.
- Grund: Zu viele Quellen erschweren Auswahl, Prüfung und Wartung.
- Kriterium: Jede Quelle hat einen Zweck im Supportfall.

### 19. Testfragen wiederverwenden
- Praxis: Testfragen wiederverwenden.
- Grund: Gleiche Fragen machen Verbesserungen sichtbar.
- Kriterium: Lab 3.3 und Lab 5.1 nutzen ein gemeinsames Testlog.

### 20. Fallbacks offen begrenzen
- Praxis: Fallbacks offen begrenzen.
- Grund: Demo oder Screenshot ersetzt keinen eigenen Laufzeitnachweis.
- Kriterium: Protokoll nennt die verbleibende Einschränkung.

## Studio-Agent und Skills

### 21. Build-Komponenten einzeln prüfen
- Praxis: Build-Komponenten einzeln prüfen.
- Grund: Fehler in Instructions, Knowledge, Tools oder Skills sehen ähnlich aus.
- Kriterium: Preview wird nach jedem Baustein genutzt.

### 22. Skills klein halten
- Praxis: Skills klein halten.
- Grund: Große Skills werden schwer auszulösen, zu prüfen und zu warten.
- Kriterium: Ein Skill löst eine klar benannte Teilaufgabe.

### 23. Skill-Beschreibung schärfen
- Praxis: Skill-Beschreibung schärfen.
- Grund: Die Beschreibung entscheidet über Auslösung stärker als schöne Langtexte.
- Kriterium: Trigger-Test zeigt, wann der Skill geladen wird.

### 24. Progressive Disclosure nutzen
- Praxis: Progressive Disclosure nutzen.
- Grund: Agenten benötigen nicht jedes Detail im Hauptprompt.
- Kriterium: Spezialwissen liegt im Skill und wird bedarfsgerecht geladen.

### 25. Generate-with-AI-Ergebnis kontrollieren
- Praxis: Generate-with-AI-Ergebnis kontrollieren.
- Grund: Automatisch erzeugte Skills brauchen fachliche und sicherheitliche Prüfung.
- Kriterium: Vor Nutzung sind Zweck, Grenzen und Ausgabeformat geprüft.

## Tools und MCP

### 26. Mit lesenden Tools beginnen
- Praxis: Mit lesenden Tools beginnen.
- Grund: Read-only senkt Nebenwirkungen und macht Toolaufrufe beobachtbar.
- Kriterium: Erster Tooltest verändert keine Kursdaten.

### 27. Tool-Beschreibung als Steuerfläche behandeln
- Praxis: Tool-Beschreibung als Steuerfläche behandeln.
- Grund: Die Orchestrierung nutzt Beschreibungen zur Auswahl.
- Kriterium: Beschreibung nennt Zweck, Zeitpunkt und Grenzen.

### 28. DLP-Blocker als Lernsignal nutzen
- Praxis: DLP-Blocker als Lernsignal nutzen.
- Grund: Blockierte Tools zeigen reale Governance statt Kursfehler.
- Kriterium: Fallback dokumentiert Richtlinie und Auswirkung.

### 29. MCP-Betreiber und Zugriff prüfen
- Praxis: MCP-Betreiber und Zugriff prüfen.
- Grund: MCP erweitert Tool- und Datenzugriff über externe Server.
- Kriterium: Server, Authentifizierung, Tools und Resources sind dokumentiert.

### 30. Connected Agents als Ausblick begrenzen
- Praxis: Connected Agents als Ausblick begrenzen.
- Grund: Zusätzliche Agenten erhöhen Komplexität und Verantwortungsfragen.
- Kriterium: Im Kurs bleibt der Fokus auf MCP und Toollauf.

## Evaluation und Qualität

### 31. Preview und Evaluate unterscheiden
- Praxis: Preview und Evaluate unterscheiden.
- Grund: Preview prüft Einzelfälle; Evaluate macht Testsets wiederholbar.
- Kriterium: Qualitätsaussage nennt Prüfmodus und Grenze.

### 32. Grenzfälle ins Testset aufnehmen
- Praxis: Grenzfälle ins Testset aufnehmen.
- Grund: Nur Standardfragen überdecken Eskalations- und Zuständigkeitsfehler.
- Kriterium: Testset enthält normale Fälle, Grenzen, Skill- und Toolfragen.

### 33. Schwächste Antwort zuerst verbessern
- Praxis: Schwächste Antwort zuerst verbessern.
- Grund: Kleine gezielte Änderungen bringen mehr als breite Prompt-Umbauten.
- Kriterium: Nachbesserung ist auf Fehlerursache zurückgeführt.

### 34. Monitor nicht vor Nutzung überbewerten
- Praxis: Monitor nicht vor Nutzung überbewerten.
- Grund: Betriebsdaten entstehen erst nach veröffentlichter Nutzung.
- Kriterium: Vor Pilotbetrieb liegen Tests, aber keine falsche Monitor-Gewissheit vor.

### 35. Keine Produktreife aus einem grünen Test ableiten
- Praxis: Keine Produktreife aus einem grünen Test ableiten.
- Grund: Testsets sind Stichproben, keine Zertifizierung.
- Kriterium: Governance-Kurzcheck bleibt erforderlich.

## Veröffentlichung und Workflow

### 36. Publish nicht mit Speichern verwechseln
- Praxis: Publish nicht mit Speichern verwechseln.
- Grund: Kanalnutzer sehen Änderungen erst nach Veröffentlichung und neuer Session.
- Kriterium: Publish-Protokoll enthält Version und Testkanal.

### 37. Freigabeziel klein halten
- Praxis: Freigabeziel klein halten.
- Grund: Pilotgruppen reduzieren Oversharing und Supportlast.
- Kriterium: Teams-Test läuft mit Kurs- oder Pilotgruppe.

### 38. Workflow deterministisch halten
- Praxis: Workflow deterministisch halten.
- Grund: Wiederholbare Aktionen gehören in Flows, offene Entscheidungen in den Agenten.
- Kriterium: Ticketanlage folgt festen Feldern und Freigabeschritt.

### 39. Response an den Agenten einplanen
- Praxis: Response an den Agenten einplanen.
- Grund: Agent-Flows brauchen eine klare Rückmeldung an den Agenten.
- Kriterium: Workflow liefert Status oder Ticketnummer zurück.

### 40. Erneut veröffentlichen nach Tooländerung
- Praxis: Erneut veröffentlichen nach Tooländerung.
- Grund: Neue Tools und Workflows müssen im Kanal aktiv werden.
- Kriterium: Nach Workflow-Anbindung erfolgt erneuter Publish-Check.

## Sicherheit, Betrieb und Transfer

### 41. Nur fiktive Kursdaten verwenden
- Praxis: Nur fiktive Kursdaten verwenden.
- Grund: Reale Daten erzeugen Datenschutz-, Compliance- und Vertrauensrisiken.
- Kriterium: Prompts, Quellen und Logs enthalten ausschließlich Nordwind-Daten.

### 42. Credit-Verantwortung vorab klären
- Praxis: Credit-Verantwortung vorab klären.
- Grund: Unbegrenztes Testen kann Kosten verursachen.
- Kriterium: Limit, Zuständige und Testumfang sind benannt.

### 43. Pilotverantwortung benennen
- Praxis: Pilotverantwortung benennen.
- Grund: Ohne Owner veralten Agenten, Skills und Quellen.
- Kriterium: Aktionsplan enthält Verantwortlichkeit und Review-Termin.

### 44. Abschaltkriterium definieren
- Praxis: Abschaltkriterium definieren.
- Grund: Ein Pilot braucht eine Grenze für Qualität, Kosten oder Risiko.
- Kriterium: Governance-Kurzcheck enthält Stoppsignal.

### 45. Vor Kurs UI und Preview prüfen
- Praxis: Vor Kurs UI und Preview prüfen.
- Grund: Copilot Studio ändert sich tenant- und rolloutsensitiv.
- Kriterium: Klickpfade werden nicht als garantiert formuliert.
