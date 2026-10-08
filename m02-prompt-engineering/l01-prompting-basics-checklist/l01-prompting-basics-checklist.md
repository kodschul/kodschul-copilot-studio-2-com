# Lab 2.1 – Prompt-Checkliste

Ein Prompt entscheidet, was ein Modell aus seinem Kontext macht. Dieses Lab vergleicht einen schlechten und einen besseren Supportprompt für den späteren Nordwind IT-Helfer.

## Vier Bausteine

| Baustein | Prüffrage | Support-Beispiel |
| --- | --- | --- |
| Rolle | Aus welcher Perspektive antwortet das Modell? | interner IT-Support für Nordwind |
| Kontext | Welche Fakten und Quellen gelten? | IT-Richtlinie und Onboarding-Leitfaden |
| Aufgabe | Was soll konkret entstehen? | Standardfrage beantworten oder eskalieren |
| Format | Wie soll die Antwort aussehen? | kurz, in Schritten, mit Kontaktweg |

## 6-Punkte-Checkliste

| # | Punkt | Prüffrage |
| --- | --- | --- |
| 1 | Klarheit | Ist die Aufgabe eindeutig formuliert? |
| 2 | Kontext | Sind Rolle, Zielgruppe und Quelle genannt? |
| 3 | Fokus | Ist das Hauptziel der Antwort klar? |
| 4 | Struktur | Sind Format, Länge und Reihenfolge festgelegt? |
| 5 | Sprachstil | Passt Ton und Sprachebene zum Supportfall? |
| 6 | Beispiele/Referenzen | Gibt es ein Muster oder eine Quelle als Referenz? |

> **Merksatz:** Was im Prompt fehlt, ergänzt das Modell stillschweigend; im Support kann genau diese Ergänzung riskant sein.

## Beispielprompts

**Schlechter Prompt**

```text
Beantworte IT-Fragen für Nordwind.
```

**Besserer Prompt**

```text
Rolle: Interner IT-Support für Nordwind Consulting.
Kontext: Grundlage ist die angehängte Nordwind-IT-Richtlinie. Antworte nur auf Basis dieser Informationen.
Aufgabe: Beantworte Standardfragen zu VPN, MFA, Firmengeräten und Software.
Format: Maximal fünf Stichpunkte, danach der passende Kontaktweg.
Grenzen: Keine Sonderberechtigungen, Vertrags- oder Gehaltsfragen entscheiden.
Eskalation: Ist die Frage nicht durch die Quelle abgedeckt oder verlangt sie eine Ausnahme, an das IT-Ticket-Portal beziehungsweise HR verweisen.
```

## Übung: beide Prompts vergleichen

Voraussetzung: Copilot Chat; die Datei [nordwind-it-richtlinie.md](../../project/nordwind-it-richtlinie.md) wird in beiden Durchläufen angehängt. Die Übung verändert die Projektbasis nicht.

Testfragen:

- **Frage A:** „Wie richte ich VPN ein, und was mache ich, wenn es nicht klappt?“
- **Frage B:** „Kann ich mir Zugriff auf die Projektablage eines anderen Teams selbst freischalten?“

Aufgaben:

1. Den schlechten Prompt zusammen mit Frage A und danach mit Frage B ausführen; beide Antworten notieren.
2. Den besseren Prompt zusammen mit Frage A und danach mit Frage B ausführen; beide Antworten notieren.
3. Die Antworten in einer Tabelle vergleichen: Quellenbezug, Struktur, Grenze/Eskalation.
4. Den Checklistenpunkt benennen, der den größten Unterschied gemacht hat.

Checkpoint: Je Prompt liegen zwei Antworten vor, und die Vergleichstabelle nennt mindestens zwei Unterschiede.

Fallback ohne Copilot-Zugriff: Die Beispielantworten unten lesen und die Tabelle daran ausfüllen. Einschränkung: Die Modellwirkung wird nicht selbst beobachtet.

## Beispielergebnis

Der Wortlaut variiert zwischen Läufen; ein typisches Muster sieht so aus:

| Kriterium | Schlechter Prompt | Besserer Prompt |
| --- | --- | --- |
| Quellenbezug | allgemeine VPN-Hinweise, Quelle nicht erkennbar | Cisco Secure Client, Verbindungsziel und MFA aus der Richtlinie |
| Struktur | Fließtext, Länge schwankt | höchstens fünf Stichpunkte plus Kontaktweg |
| Grenze/Eskalation (Frage B) | gibt allgemeine Tipps zur Rechtevergabe | verweist an das IT-Ticket-Portal, entscheidet nichts selbst |
| Nutzbarkeit | generisch | direkt als Supportantwort verwendbar |

Größte Verbesserung: Die Kombination aus Quellenbindung (Kontext) und Eskalationsregel verhindert, dass der Prompt Ausnahmen oder nicht belegte Fakten erfindet.

## Fazit

- Rolle, Kontext, Aufgabe und Format bilden das Grundgerüst; die Checkliste macht Lücken prüfbar.
- Support-Prompts brauchen immer Grenzen und eine Eskalationsregel.
