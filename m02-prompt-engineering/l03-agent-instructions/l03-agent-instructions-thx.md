# Lab 2.3 – Vom Prompt zur Agenten-Instruktion

Dieses Lab unterscheidet einmalige Nutzerprompts von dauerhaften Agenten-Instruktionen. Ergebnis ist ein Skelett für den späteren „Nordwind IT-Helfer“.

**Leitfragen:**

<details><summary>Was gehört in eine Instruktion, was in eine Wissensquelle?</summary>

Instruktionen beschreiben Aufgabe, Verhalten, Grenzen und Ausgabe. Wissensquellen enthalten Fakten, Richtlinien und Inhalte, die sich ändern können.
</details>

<details><summary>Wie formuliert man, was der Agent nicht tun soll?</summary>

Verbote werden konkret mit Auslöser und Alternativverhalten formuliert: nicht entscheiden, sondern eskalieren oder Quelle nennen.
</details>

<details><summary>Warum reicht ein guter Chat-Prompt nicht als Agenten-Instruktion?</summary>

Ein Chat-Prompt gilt für eine Anfrage. Eine Agenten-Instruktion steuert jede Anfrage und muss daher robuster, wiederholbar und prüfbar sein.
</details>

## Begriffe

| Begriff | Bedeutung |
| --- | --- |
| Nutzerprompt | einmalige Anfrage im aktuellen Chat |
| Instruktion / System-Prompt | dauerhafte Verhaltensregel für den Agenten |
| Wissensquelle | Dokument oder Datenquelle mit Fakten für Antworten |
| Eskalation | Weiterleitung, wenn der Agent nicht sicher beantworten darf |
| Qualitätskontrolle | Prüfregel für Antwort, Quelle, Grenze und Format |

## Anatomie einer Agenten-Instruktion

| Baustein | Zweck | Nordwind-Beispiel |
| --- | --- | --- |
| Auftrag | Kernrolle und Zweck | interner IT- und Onboarding-Support |
| Arbeitsprinzipien | Stil, Quellenbindung, Annahmen | kurz, sachlich, keine Fakten erfinden |
| Schritte | Standardablauf pro Anfrage | Frage einordnen, Quelle prüfen, antworten oder eskalieren |
| Standardausgabe | Antwortformat | Kurzantwort, Schritte, Kontaktweg |
| Qualitätskontrolle | Selbstprüfung vor Antwort | Quelle vorhanden, Grenze eingehalten, Eskalation geprüft |
| Fehlerbehandlung/Eskalation | Verhalten bei Lücken und Risiken | IT-Ticket-Portal oder HR nennen |
| Beispiele | Muster für typische und kritische Fälle | VPN-Frage, Gehaltsfrage, Sonderberechtigung |

> **Merksatz:** Fakten gehören in Quellen; Verhalten, Grenzen und Prüfregeln gehören in die Instruktion.

## Was nicht in die Instruktion gehört

| Gehört in Instruktion | Gehört in Wissensquelle |
| --- | --- |
| „Antworte nur auf Basis freigegebener Nordwind-Quellen.“ | konkrete VPN-Adresse |
| „Eskalation bei Sonderberechtigungen.“ | aktuelle IT-Support-Kontaktdaten |
| „Keine Gehalts- oder Vertragsdetails beantworten.“ | Onboarding-Ablauf der ersten 30 Tage |
| „Maximal fünf Stichpunkte.“ | Passwortwechselintervall |

## Verbote gut formulieren

| Schwach | Besser |
| --- | --- |
| „Keine falschen Antworten geben.“ | „Wenn keine Quelle vorliegt, keine Antwort erfinden; fehlende Quelle benennen und eskalieren.“ |
| „Keine sensiblen Themen.“ | „Individuelle Vertrags-, Gehalts- oder Sonderberechtigungsfragen nicht beantworten; an HR oder IT-Support verweisen.“ |
| „Nicht zu lang antworten.“ | „Maximal fünf Stichpunkte plus Kontaktweg, wenn Eskalation nötig ist.“ |

## Fazit

- Eine Instruktion ist wiederverwendbare Steuerung, kein einmaliger Arbeitsauftrag.
- Wissensquellen tragen Fakten; Instruktionen tragen Verhalten und Grenzen.
- Gute Verbote nennen Auslöser, untersagte Handlung und sicheres Alternativverhalten.

Die Übung füllt ein Instruktionsskelett für den späteren Nordwind IT-Helfer aus.
