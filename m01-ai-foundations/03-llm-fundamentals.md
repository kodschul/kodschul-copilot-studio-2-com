# Wie ein Sprachmodell antwortet

Hintergrundmaterial zu Modul 1. Sprachmodelle formulieren plausibel, antworten aber nicht automatisch wahr. Entscheidend sind Token-Vorhersage, Kontext, Grounding und die Abgrenzung zum Agenten.

## Begriffe

| Begriff | Bedeutung |
| --- | --- |
| Token | Textbaustein, auf dessen Basis das Modell Fortsetzungen berechnet |
| Training | Lernphase, in der Modellgewichte aus großen Datenmengen entstehen |
| Kontext | Informationen, die während einer Anfrage mitgegeben oder gefunden werden |
| Grounding | Verankerung einer Antwort in bereitgestellten oder gefundenen Quellen |
| RAG | Retrieval Augmented Generation: Quellen suchen und für die Antwort nutzen |
| Microsoft Graph | Berechtigungs- und Kontextschicht für Microsoft-365-Inhalte |

## Antwortentstehung

```text
Prompt + Kontext + Instruktion
  → Token für Token wahrscheinliche Fortsetzung
  → Antwort mit Quellenbezug, wenn Grounding greift
  → menschliche Prüfung bei Fakten, Entscheidungen und Risiken
```

| Punkt | Konsequenz |
| --- | --- |
| Das Modell sagt wahrscheinliche Token voraus | flüssige Sprache ist kein Wahrheitsbeweis |
| Training ist nicht der Chatverlauf | eine Korrektur im Chat trainiert das Modell nicht dauerhaft |
| Kontext steuert stark | bessere Quellen und klare Grenzen verbessern Antworten |
| Grounding braucht Zugriff | fehlende Berechtigung bedeutet fehlender Kontext |

> **Merksatz:** Gute Antworten entstehen aus Modellfähigkeit plus passendem Kontext; ohne Kontext bleibt selbst ein starkes Modell allgemein.

## Copilot-Grounding im Arbeitskontext

| Frage | Einordnung |
| --- | --- |
| Welche Daten können einfließen? | Microsoft-365-Inhalte, auf die die anfragende Person berechtigt ist |
| Was passiert bei fehlender Berechtigung? | Copilot erhält diese Inhalte nicht als Kontext |
| Warum unterscheiden sich Antworten? | Personen, Verlauf, Zeitpunkt, Dateien und Berechtigungen können variieren |
| Was bleibt zu prüfen? | Zahlen, Namen, Fristen, Quellenbezug und sensible Entscheidungen |

## Prompt, Kontext, Agent

| Ebene | Zweck | Nordwind-Beispiel |
| --- | --- | --- |
| Prompt | einmalige Arbeitsanweisung | „Beantworte diese VPN-Frage kurz.“ |
| Kontext | Material für diese Antwort | IT-Richtlinie und Onboarding-Leitfaden |
| Agent | wiederverwendbare Arbeitsrolle | „Nordwind IT-Helfer“ mit festen Grenzen und Eskalationsregeln |

## Typische Fehler

- Gute Formulierung wird mit fachlicher Korrektheit verwechselt.
- Fehlender Kontext wird als Modellschwäche statt als Quellenproblem behandelt.
- Berechtigungen werden erst geprüft, nachdem Antworten unerwartet abweichen.

Angewendet in Lab 2.1, Lab 3.1 und Lab 5.1.
