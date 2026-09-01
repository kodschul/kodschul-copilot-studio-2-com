# M01 Theorie: Auftakt, KI-Landschaft & Einführungsstrategie

> Diese Seite ist als Lesetext für die Teilnehmenden (TN) gedacht und dient dem Trainer gleichzeitig
> als Vorlage für den Showcase im Plenum. Trainer-Hinweise sind gesondert im Abschnitt
> "Trainer-Showcase" markiert.

## Lernziel

Nach diesem Modul könnt ihr die eigene Softwarelandschaft einordnen, ChatGPT/Claude/Copilot
unterscheiden und Optionen zur KI-Einführung im Unternehmen bewerten.

## Dauer

Tag 1 · 09:00–10:30 · 90 Minuten

## Zielbild dieser Schulung

Nach den 2 Tagen habt ihr selbst einen Agenten gebaut, der aus Plänen Daten zieht und automatisiert
weitergibt. Die Schulung ist entlang von zwei konkreten EFG-Anwendungsfällen aufgebaut:

1. **Datenextraktion aus Plänen (PDF/DXF) → Solarcomputer:** Flächen-/Mengendaten automatisiert
   extrahieren und ins Heizlastprogramm übernehmen.
2. **Aufmaßprüfung:** Massenaufstellungen gegen Pläne prüfen (Soll/Ist-Abgleich).

## Softwarelandschaft im Ingenieurbüro

Bevor man KI sinnvoll einsetzt, lohnt sich ein Blick auf die eigene Softwarelandschaft: welche Systeme
sind im Einsatz (M365/Outlook/Teams, CAD/DXF-Software, Solarcomputer, Ablage/SharePoint), und wo werden
Daten heute manuell zwischen ihnen übertragen? Genau an diesen "Medienbrüchen" setzen KI-Agenten
sinnvoll an — deshalb ist der erste Schritt in dieser Schulung immer, den eigenen Ist-Zustand
transparent zu machen, bevor über Technologie gesprochen wird. → Übung siehe [uebung.md](uebung.md), Aufgabe 1.

## LLM-Landschaft: ChatGPT, Claude, Copilot

- **Modell** = die KI-„Engine" im Hintergrund (z. B. GPT-5, Claude, Gemini). **Produkt** = die Anwendung, in der man sie nutzt.
- **ChatGPT** (OpenAI): eigenständiges Produkt, sehr breit einsetzbar, aber ohne besondere Anbindung an Firmendaten.
- **Claude** (Anthropic): eigenständiges Produkt, stark bei Text/Code, ebenfalls ohne Standard-Anbindung an M365.
- **Copilot** (Microsoft): Produktfamilie, tief in M365 integriert (Outlook, Teams, SharePoint) — deshalb naheliegend für EFG, da M365 Business bereits vorhanden ist.

Welches Modell im Hintergrund läuft, ist für den Alltag fast egal — entscheidend ist, in welchem
Produkt man arbeitet und ob es an die eigenen Daten/Systeme andockt.

## Wie führt ein Unternehmen KI ein? Optionen & Abwägungen

| Option                                       | Beschreibung                            | Passt gut wenn...                         |
| -------------------------------------------- | --------------------------------------- | ----------------------------------------- |
| Fertige KI-Tools nutzen (z. B. Copilot Chat) | Sofort einsatzbereit, kein Bau nötig    | Schneller Einstieg, generische Aufgaben   |
| Eigene Agenten bauen (Copilot Studio)        | Auf eigene Prozesse/Daten zugeschnitten | Wiederkehrende, spezifische Prozesse      |
| Pilotprojekt in einem Team                   | Risikoarm, schnelles Lernen             | Neues Thema, unklare Erfolgsaussicht      |
| Unternehmensweiter Rollout                   | Größerer Hebel, mehr Abstimmungsaufwand | Erprobtes Vorgehen, klare Anwendungsfälle |

Wichtige Abwägungskriterien sind Datenschutz/Datensicherheit, Kosten/Lizenzen, Kontrolle &
Nachvollziehbarkeit, Pflegeaufwand und vorhandenes Know-how im Team. → Übung siehe [uebung.md](uebung.md), Aufgabe 2.

## Optionen für Prozessoptimierung im Überblick

| Ansatz                                          | Beispiel                                   | Wann sinnvoll                                       |
| ----------------------------------------------- | ------------------------------------------ | --------------------------------------------------- |
| Reine Automatisierung (Power Automate, ohne KI) | Datei wird automatisch kopiert             | Regeln sind fest, keine Interpretation nötig        |
| KI-gestützte Assistenz (Copilot Chat)           | Text zusammenfassen                        | Mensch bleibt im Loop                               |
| KI-Agent (Copilot Studio + Power Automate)      | Plan lesen, Wert automatisiert weitergeben | Wiederkehrender Prozess mit "Verstehen" + "Handeln" |

Beide EFG-Use-Cases sind klare Agenten-Fälle, da "Verstehen" und "Handeln" kombiniert werden.

## Trainer-Showcase

- **Begrüßung & Zielbild (10 Min):** Vorstellungsrunde (Name, Rolle, Erwartung an die 2 Tage), danach
  das Zielbild oben im Plenum vorlesen/zeigen und kurz auf beide EFG-Use-Cases verweisen.
- **Softwarelandschaft (20 Min):** Gemeinsam an Flipchart/Whiteboard die Systeme und Medienbrüche der
  Gruppe sammeln, bevor die TN in Übung 1 selbst arbeiten.
- **LLM-Landschaft (20 Min):** Tabelle/Vergleich im Plenum durchgehen, Prequestion vorher stellen (siehe
  unten).
- **Einführungsoptionen (25 Min):** Tabelle Schritt für Schritt erläutern, danach in Übung 1b vertiefen.
- **Prozessoptimierung (10 Min):** Tabelle zeigen und direkten Bezug zu den beiden EFG-Use-Cases
  herstellen.
- **Prequestion (vor der LLM-Landschaft):** "Was glaubt ihr — was ist der Unterschied zwischen ChatGPT,
  Claude und Copilot?" (vor der Erklärung raten lassen)
- **Umfrage:** Stimmungsbild — "Wie weit ist KI heute schon in eurem Arbeitsalltag im Einsatz?" (1–5)

## Leitfragen

Beantwortet die Fragen zuerst selbst, bevor ihr sie aufklappt (Test-Effekt).

<details>
<summary>Was ist der Hauptunterschied zwischen einem "Modell" und einem "Produkt"?</summary>

Modell = die KI-Engine im Hintergrund (z. B. GPT, Claude, Gemini). Produkt = die Anwendung, in der man
das Modell nutzt (z. B. ChatGPT, Copilot). Welches Modell im Hintergrund läuft, ist für den Alltag fast
egal — entscheidend ist, in welchem Produkt man arbeitet und ob es an die eigenen Daten/Systeme andockt.

</details>

<details>
<summary>Warum ist Copilot für EFG naheliegend, obwohl ChatGPT/Claude ähnliche Modelle nutzen?</summary>

Weil EFG bereits M365 Business lizenziert hat und Copilot tief in Outlook/Teams/SharePoint integriert
ist — dadurch entfällt eine separate Anschaffung und die Anbindung an bestehende Daten ist einfacher.

</details>

<details>
<summary>Nennt ein Kriterium, das bei der KI-Einführung in einem Unternehmen wichtig ist.</summary>

Z. B. Datenschutz/Datensicherheit, Kosten/Lizenzen, Kontrolle & Nachvollziehbarkeit, Pflegeaufwand oder
vorhandenes Know-how im Team.

</details>

<details>
<summary>Ordnet zu: "Datei wird automatisch kopiert" — welcher Ansatz aus der Prozessoptimierungs-Tabelle passt?</summary>

Reine Automatisierung (Power Automate ohne KI) — feste Regeln, keine Interpretation nötig.

</details>
