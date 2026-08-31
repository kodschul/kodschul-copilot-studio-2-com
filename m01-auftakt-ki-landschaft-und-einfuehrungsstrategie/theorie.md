# M01 Theorie: Auftakt, KI-Landschaft & Einführungsstrategie

## Lernziel

Die eigene Softwarelandschaft einordnen, ChatGPT/Claude/Copilot unterscheiden und Optionen zur
KI-Einführung im Unternehmen bewerten können.

## Dauer

Tag 1 · 09:00–10:30 · 90 Minuten

## Begrüßung & Zielbild (10 Min)

- Vorstellungsrunde (Name, Rolle, Erwartung an die 2 Tage)
- Zielbild zeigen: "Nach 2 Tagen habt ihr selbst einen Agenten gebaut, der aus Plänen Daten zieht und automatisiert weitergibt."
- Kurz auf beide EFG-Use-Cases verweisen (Datenextraktion → Solarcomputer, Aufmaßprüfung).

## Softwarelandschaft im Ingenieurbüro (20 Min)

Gemeinsam sammeln: welche Systeme nutzt EFG heute (M365/Outlook/Teams, CAD/DXF-Software, Solarcomputer,
Ablage/SharePoint)? Wo werden Daten manuell zwischen Systemen übertragen? Genau an diesen
"Medienbrüchen" setzen KI-Agenten sinnvoll an. → Übung siehe [uebung.md](uebung.md), Aufgabe 1.

## LLM-Landschaft: ChatGPT, Claude, Copilot (20 Min)

- **Modell** = die KI-„Engine" im Hintergrund (z. B. GPT-5, Claude, Gemini). **Produkt** = die Anwendung, in der man sie nutzt.
- **ChatGPT** (OpenAI): eigenständiges Produkt, sehr breit einsetzbar, aber ohne besondere Anbindung an Firmendaten.
- **Claude** (Anthropic): eigenständiges Produkt, stark bei Text/Code, ebenfalls ohne Standard-Anbindung an M365.
- **Copilot** (Microsoft): Produktfamilie, tief in M365 integriert (Outlook, Teams, SharePoint) — deshalb naheliegend für EFG, da M365 Business bereits vorhanden ist.

## Wie führt ein Unternehmen KI ein? Optionen & Abwägungen (25 Min)

| Option | Beschreibung | Passt gut wenn... |
| --- | --- | --- |
| Fertige KI-Tools nutzen (z. B. Copilot Chat) | Sofort einsatzbereit, kein Bau nötig | Schneller Einstieg, generische Aufgaben |
| Eigene Agenten bauen (Copilot Studio) | Auf eigene Prozesse/Daten zugeschnitten | Wiederkehrende, spezifische Prozesse |
| Pilotprojekt in einem Team | Risikoarm, schnelles Lernen | Neues Thema, unklare Erfolgsaussicht |
| Unternehmensweiter Rollout | Größerer Hebel, mehr Abstimmungsaufwand | Erprobtes Vorgehen, klare Anwendungsfälle |

Abwägungskriterien: Datenschutz/Datensicherheit, Kosten/Lizenzen, Kontrolle & Nachvollziehbarkeit,
Pflegeaufwand, vorhandenes Know-how im Team. → Übung siehe [uebung.md](uebung.md), Aufgabe 2.

## Optionen für Prozessoptimierung im Überblick (10 Min)

| Ansatz | Beispiel | Wann sinnvoll |
| --- | --- | --- |
| Reine Automatisierung (Power Automate, ohne KI) | Datei wird automatisch kopiert | Regeln sind fest, keine Interpretation nötig |
| KI-gestützte Assistenz (Copilot Chat) | Text zusammenfassen | Mensch bleibt im Loop |
| KI-Agent (Copilot Studio + Power Automate) | Plan lesen, Wert automatisiert weitergeben | Wiederkehrender Prozess mit "Verstehen" + "Handeln" |

Beide EFG-Use-Cases sind klare Agenten-Fälle, da "Verstehen" und "Handeln" kombiniert werden.

## Leitfragen

Lies die Fragen bevor du sie im Plenum auflöst.

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
