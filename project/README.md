# Nordwind Consulting – Kursprojekt

Ein anonymisiertes Beispielunternehmen zieht sich durch beide Kurstage: **Nordwind Consulting**.
Alle Daten sind fiktiv. Gebaut wird der interne IT- und Onboarding-Support-Agent **„Nordwind IT-Helfer"**.

Dieser Ordner bündelt die Dateien, die mehrere Labs nutzen. Jede Übung nennt nur die Dateien, die sie braucht.

## Wie sich das Projekt aufbaut

| Tag | Lab | Ergebnis | Datei(en) hier |
| --- | --- | --- | --- |
| 1 | 2.3 | Instruktions-Skelett für den IT-Helfer | – (entsteht im Lab) |
| 1 | 3.3 | Erster Chat-Agent ohne Wissensquelle + Testprotokoll | – |
| 1 | 4.1–4.3 | Use-Case-Canvas, Architektur-Kurzkonzept, System-Prompt, `SKILL.md` | – |
| 2 | 5.1 | Chat-Agent mit Wissensquellen, Vorher/Nachher-Vergleich | `nordwind-it-richtlinie.md`, `nordwind-onboarding-leitfaden.md` |
| 2 | 6.1–6.2 | Copilot-Studio-Agent (GitHub-Copilot-Harness) mit Skills | dieselben Wissensquellen |
| 2 | 7.1 | Lesendes Konnektor-Tool auf SharePoint-Liste `IT-Geräte` | `nordwind-it-geraete.md` |
| 2 | 7.2–7.3 | MCP-Tool und Testset | – |
| 2 | 8.1–8.2 | In Teams veröffentlichter Agent mit Workflow „Support-Ticket" | – |
| 2 | 8.3 | Governance-Kurzcheck und persönlicher Aktionsplan | – |

## Vorhandene Dateien

| Datei | Inhalt | Genutzt in |
| --- | --- | --- |
| `nordwind-it-richtlinie.md` | VPN, Geräte- und Passwortrichtlinie, IT-Support-Kontakt | Wissensquelle ab Lab 5.1 |
| `nordwind-onboarding-leitfaden.md` | erster Arbeitstag, erste 30 Tage, häufige Fragen | Wissensquelle ab Lab 5.1 |
| `nordwind-it-geraete.md` | Beispielinhalt für die SharePoint-Liste `IT-Geräte` | Lab 7.1 |

Zwischenstände aus den Labs (Testprotokoll, System-Prompt, `SKILL.md`, Testset) werden lokal oder in
der Kursablage gespeichert, damit Tag 2 darauf aufbauen kann.
