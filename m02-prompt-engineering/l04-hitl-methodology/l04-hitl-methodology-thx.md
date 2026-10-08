# Lab 2.4 – Human-in-the-Loop

Dieses Lab nutzt Human-in-the-Loop als Methode für das Design des Support-Agenten. Entscheidungen bleiben beim Menschen, während Copilot beim Strukturieren und Ausformulieren hilft.

**Leitfragen:**

<details><summary>An welchen Stellen muss der Mensch zwingend entscheiden?</summary>

Bei Zielgruppe, erlaubten Themen, Grenzen, Eskalation und Qualitätsmaßstab. Das Modell kann Vorschläge liefern, entscheidet aber nicht die Verantwortung.
</details>

<details><summary>Warum ist ein One-Shot-Prompt für Agentendesign riskant?</summary>

Der Prompt überlässt Kernentscheidungen dem Modell: Zweck, Grenzen, Datenlage und Eskalation können dann plausibel, aber falsch gesetzt werden.
</details>

<details><summary>Wie passt HITL zum Nextise Agentic Way?</summary>

HITL trennt Problem, Konzept und Umsetzung. Jede Stufe erhält eine menschliche Prüfung vor dem nächsten Artefakt.
</details>

## Vier Schritte

| Schritt | Mensch entscheidet | Copilot unterstützt |
| --- | --- | --- |
| Vision | Zielgruppe und Nutzen des Support-Agenten | Formulierungen schärfen |
| Gliederung | welche Fragen, Themen und Grenzen wichtig sind | Strukturvorschläge machen |
| Kerninhalte | je Bereich die verbindliche Aussage festlegen | Lücken sichtbar machen |
| Scaffold | geprüftes Gerüst in Instruktion oder Konzept überführen | Textentwurf erstellen |

> **Merksatz:** HITL bedeutet nicht „KI fragt zwischendurch“, sondern „menschliche Entscheidungen bleiben an den kritischen Übergaben verbindlich“.

## One-Shot vs. HITL

| Ansatz | Ergebnisrisiko | Passender Einsatz |
| --- | --- | --- |
| One-Shot | Zielgruppe, Grenzen und Eskalation werden vom Modell geraten | grober Ideensammler |
| HITL | Entscheidungen entstehen schrittweise und prüfbar | Agentendesign, Supportprozesse, Governance |

## Support-Agent als Designfall

| Entscheidung | Prüffrage |
| --- | --- |
| Zielgruppe | Wer stellt Fragen und in welchem Moment? |
| Fragen | Welche Standardfragen deckt der Agent sicher ab? |
| Grenzen | Welche Themen darf der Agent nicht beantworten? |
| Eskalation | Wann geht es an IT-Support, HR oder eine Führungskraft? |
| Belege | Welche Wissensquelle deckt jede Antwort ab? |

## Verbindung zu Prompt-Techniken

| HITL-Schritt | Nützliche Technik |
| --- | --- |
| Vision | Zero-Shot zum Schärfen von Alternativen |
| Gliederung | Chain-of-Thought für sichtbare Strukturentscheidungen |
| Kerninhalte | ReAct, wenn Quellenstellen geprüft werden |
| Scaffold | Few-Shot, wenn ein Zielformat existiert |

## Grenzen

- Für sehr kleine Einmalfragen ist HITL zu schwergewichtig.
- Eine ungeprüfte Gliederung ist kein HITL, sondern One-Shot mit Zwischenstation.
- HITL verhindert keine falschen Quellen; Quellen müssen separat geprüft werden.

## Fazit

- Agentendesign braucht menschliche Entscheidungen zu Zielgruppe, Fragen, Grenzen und Eskalation.
- Copilot ist stark beim Vorschlagen, Sortieren und Ausformulieren.
- HITL macht Übergaben prüfbar und bereitet die Drei-Assistenten-Kette vor.

Die Übung erstellt eine HITL-Gliederung für den Nordwind IT-Helfer.
