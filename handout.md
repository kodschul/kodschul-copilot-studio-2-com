# KI-Agenten mit Microsoft Copilot Studio & Power Automate
## Handout für Teilnehmer — EFG Engineering Facility Group

> Dieses Handout fasst die wichtigsten Inhalte der 2-tägigen Schulung zusammen.
> Ausführliche Schritt-für-Schritt-Anleitungen findest du im Trainer-Guide (auf Anfrage).

---

## Agenda im Überblick

**Tag 1 — Einordnung & Grundlagen**

| Zeit | Modul |
| --- | --- |
| 09:00–10:30 | Auftakt, KI-Landschaft & Einführungsstrategie |
| 10:45–12:15 | Grundlagen KI-Agenten |
| 13:15–14:45 | Copilot Studio im Überblick |
| 15:00–16:15 | Power Platform im Überblick |
| 16:15–17:00 | Use-Case-Discovery Workshop |

**Tag 2 — Copilot Studio in der Praxis**

| Zeit | Modul |
| --- | --- |
| 09:00–10:30 | Recap & Aufbau eines einfachen Agenten |
| 10:45–12:15 | Use Case 1: Datenextraktion aus Plänen |
| 13:15–14:45 | Automatisierung mit Power Automate |
| 15:00–16:15 | Use Case 2: Aufmaßprüfung |
| 16:15–17:00 | Wrap-up, Erweiterung & Übergabe |

## Tag 1 — Einordnung & Grundlagen

### Softwarelandschaft im Ingenieurbüro
Bevor man KI sinnvoll einsetzt, lohnt sich ein Blick auf die eigene Softwarelandschaft: welche Systeme
sind im Einsatz (M365, CAD/DXF-Tools, Solarcomputer, Ablage), und wo werden Daten heute manuell
zwischen ihnen übertragen? Genau an diesen "Medienbrüchen" setzen KI-Agenten sinnvoll an.

### KI-Landschaft: ChatGPT, Claude, Copilot im Vergleich
- **Modell** = die KI-„Engine" im Hintergrund (z. B. GPT, Claude, Gemini). **Produkt** = die Anwendung, in der man sie nutzt.
- **ChatGPT** (OpenAI): eigenständiges Produkt, sehr breit einsetzbar, aber ohne besondere Anbindung an Firmendaten.
- **Claude** (Anthropic): eigenständiges Produkt, stark bei Text/Code, ebenfalls ohne Standard-Anbindung an M365.
- **Copilot** (Microsoft): Produktfamilie, tief in M365 integriert (Outlook, Teams, SharePoint) — deshalb naheliegend für EFG, da M365 Business bereits vorhanden ist.

### Wie führt man KI im Unternehmen ein? Optionen & Abwägungen
| Option | Passt gut wenn... |
| --- | --- |
| Fertige KI-Tools nutzen (Copilot Chat) | schneller Einstieg, generische Aufgaben |
| Eigene Agenten bauen (Copilot Studio) | wiederkehrender, spezifischer Prozess |
| Pilotprojekt in einem Team | neues Thema, unklare Erfolgsaussicht |
| Unternehmensweiter Rollout | erprobtes Vorgehen, klare Use Cases |

Wichtige Abwägungskriterien: Datenschutz/Datensicherheit, Kosten/Lizenzen, Kontrolle & Nachvollziehbarkeit,
Pflegeaufwand, vorhandenes Know-how im Team.

### Optionen für Prozessoptimierung: Automatisierung vs. Assistenz vs. Agenten
| Ansatz | Beispiel | Wann sinnvoll |
| --- | --- | --- |
| Reine Automatisierung (Power Automate ohne KI) | Datei automatisch kopieren | feste Regeln, keine Interpretation nötig |
| KI-Assistenz (Copilot Chat) | Text zusammenfassen | Mensch bleibt im Loop |
| KI-Agent (Copilot Studio + Power Automate) | Plan lesen & Daten weitergeben | "Verstehen" + "Handeln" nötig |

### Was ist ein Agent?
Ein KI-System, das eine Aufgabe versteht, selbst entscheidet, welche Schritte/Werkzeuge nötig sind, und
diese ausführt — im Unterschied zum Chatbot handelt ein Agent, statt nur zu antworten.

### Was ist ein Skill / ein Tool?
Eine konkrete Fähigkeit, die ein Agent bei Bedarf aufruft (z. B. „Datei lesen", „Flow in Power Automate
auslösen"). Der Agent entscheidet selbst, wann er welches Tool braucht.

### Was ist ein Prompt?
Die Anweisung an den Agenten. Unterschieden wird zwischen dem **Nutzer-Prompt** (einzelne Anfrage) und den
**Instruktionen** (fest hinterlegter System-Prompt, der jede Anfrage begleitet).

### Prompt-Techniken
- **Kontext geben** — relevante Infos mitliefern
- **Rolle zuweisen** — z. B. „Du bist ein Assistent für Gebäudetechnik-Aufmaße"
- **Beispiele geben** — gewünschtes Ausgabeformat zeigen
- **Schritt-für-Schritt anweisen** — komplexe Aufgaben in Teilschritte zerlegen

### Copilot Studio im Überblick
Ein Agent besteht aus: **Instruktionen** (System-Prompt), **Wissen** (Knowledge-Quellen), **Tools/Skills**,
**Themen** und einem **Testfenster**. Tools können vordefinierte Konnektoren nutzen oder einen eigenen
Power-Automate-Flow auslösen. Grundprinzip: Copilot Studio „versteht", Power Automate „handelt".

### Power Platform im Überblick
- **Power Automate (Cloud):** Trigger (Auslöser) → Aktion (was passiert) über Connectors (Verbindung zu Systemen)
- **Power Automate Desktop:** für ältere Desktop-Anwendungen ohne Cloud-Connector (relevant, falls Solarcomputer keinen direkten Connector hat)
- Mit M365 Business ist die Basisnutzung beider Werkzeuge bereits enthalten

### Use-Case-Discovery: unsere EFG-Anwendungsfälle
1. **Datenextraktion aus Plänen (PDF/DXF) → Solarcomputer:** Flächen-/Mengendaten automatisiert extrahieren und ins Heizlastprogramm übernehmen.
2. **Aufmaßprüfung:** Massenaufstellungen gegen Pläne prüfen (Soll/Ist-Abgleich).

## Tag 2 — Copilot Studio in der Praxis

### Aufbau eines Agenten — Schritt für Schritt
1. Neuen Agenten anlegen, Name & Beschreibung vergeben
2. Instruktionen schreiben (Rolle, Sprache, gewünschtes Ausgabeformat)
3. Tool hinzufügen und konfigurieren
4. Im Testfenster ausprobieren und iterativ verbessern

### Use Case 1: Datenextraktion aus Plänen (PDF/DXF) → Solarcomputer
- PDF-Pläne sind der Hauptfall bei EFG, DXF (strukturiert) liefert tendenziell zuverlässigere Ergebnisse
- Zielformat: Tabelle mit Raum/Bauteil, Fläche, Einheit, Plan-Referenz
- Wichtig: Ergebnis ist eine Arbeitserleichterung mit Prüfschritt, kein fehlerfreier Autopilot

### Automatisierung mit Power Automate
- Flow nimmt die strukturierte Tabelle vom Agenten entgegen und schreibt sie z. B. in Excel/SharePoint
- Anbindung an Solarcomputer: direkter Connector (falls vorhanden), sonst Zwischenschritt über Excel/SharePoint oder Power Automate Desktop

### Use Case 2: Aufmaßprüfung
- Massenaufstellung (Soll) wird gegen die aus Plänen extrahierten Werte (Ist) abgeglichen
- Ergebnis dieser Schulung: Konzept-Skizze, kein fertiger Agent — nächster Schritt wäre ein Pilotprojekt

### Wie geht es weiter? Eigenständig erweitern
- Neue Skills/Tools nach dem gleichen Muster ergänzen wie in der Schulung gezeigt
- Bei Problemen: Testfenster-Verlauf in Copilot Studio bzw. Ausführungsverlauf in Power Automate prüfen
- Empfohlener nächster Schritt: Pilotprojekt mit echten Testdaten, Solarcomputer-Anbindung mit IT/Microsoft-Partner klären

## Glossar

| Begriff | Erklärung |
| --- | --- |
| Agent | KI-System, das eine Aufgabe versteht, Schritte plant und mithilfe von Tools ausführt |
| Skill | Eine dem Agenten zugeordnete Fähigkeit/Funktion (Synonym zu Tool im aktuellen Copilot-Studio-Konzept) |
| Tool | Konkrete Fähigkeit, die ein Agent aufruft, z. B. ein Konnektor oder ein Power-Automate-Flow |
| Prompt | Anweisung/Eingabe an den Agenten (Nutzer-Prompt oder fest hinterlegte Instruktionen) |
| Connector | Verbindung zwischen Power Automate und einem System/einer App |
| Flow | Ein in Power Automate erstellter automatisierter Ablauf aus Trigger und Aktionen |
| Trigger | Das Ereignis, das einen Flow startet |
| LLM | Large Language Model — das KI-Sprachmodell im Hintergrund eines KI-Produkts |
| ChatGPT | KI-Produkt von OpenAI, nutzt GPT-Modelle |
| Claude | KI-Produkt von Anthropic |
| Copilot | KI-Produktfamilie von Microsoft, tief in M365 integriert |

## Weiterführende Links
- https://copilotstudio.microsoft.com/
- https://make.powerautomate.com/
