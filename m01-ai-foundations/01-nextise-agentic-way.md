# The Nextise Agentic Way — Kursleitbild

Hintergrundmaterial zu Modul 1. Der Kurs nutzt KI, um KI-Lösungen zu entwerfen, zu prüfen und kontrolliert zu bauen.

## Kursrahmen

| Aspekt | Bedeutung im Kurs |
| --- | --- |
| Dauer | 2 Tage mit gemeinsamem Nordwind-Szenario |
| Ziel | von KI-Grundlagen zu einem geprüften Support-Agenten |
| Arbeitsweise | kurze Inputs, konkrete Artefakte, menschliche Prüfung |
| Wiederverwendung | Ergebnisse aus frühen Labs werden später weiterverarbeitet |

## Denkwechsel

| Alte Sicht | Agentische Sicht |
| --- | --- |
| KI beantwortet einzelne Fragen | KI unterstützt einen mehrstufigen Arbeitsprozess |
| Prompt beschreibt direkt die gewünschte Lösung | Prompt oder Instruktion beschreibt Ziel, Grenzen und Prüfkriterien |
| Mensch korrigiert am Ende | Mensch entscheidet an jedem Übergabepunkt |
| Ergebnis ist ein Text | Ergebnis ist ein nutzbares Artefakt für den nächsten Schritt |

> **Merksatz:** Agentisches Arbeiten delegiert nicht die Verantwortung, sondern strukturiert Arbeit so, dass KI-Outputs prüfbar bleiben.

## Drei Schritte

```text
Problem verstehen → Lösung konzipieren → Lösung bauen
```

| Schritt | Leitentscheidung | Typisches Artefakt |
| --- | --- | --- |
| Problem verstehen | Welches wiederkehrende Problem ist wirklich relevant? | Use-Case-Canvas |
| Lösung konzipieren | Welche Bausteine, Daten und Grenzen braucht der Agent? | Architektur-Kurzkonzept |
| Lösung bauen | Welche Instruktionen, Skills und Tests machen den Agenten nutzbar? | System-Prompt, Skill-Entwurf, Testset |

## Drei-Assistenten-Kette

```text
Problem
  → Problem-Solver
  → Solution Architect
  → Skill-/System-Prompt-Generator
```

| Assistent | Aufgabe | Ergebnis |
| --- | --- | --- |
| Problem-Solver | Use Case schärfen, Nutzen und Risiken bewerten | Canvas und Top-1-Empfehlung |
| Solution Architect | Bausteine und Ablauf ableiten | Kurzkonzept und Übergabepaket |
| Skill-/System-Prompt-Generator | Instruktion und Skill-Dateien ausarbeiten | System-Prompt und `SKILL.md`-Entwürfe |

## Verankerung im Kurs

- Die Methode wird am Morgen von Tag 1 als Leitbild eingeführt.
- Die vollständige Drei-Assistenten-Kette läuft am Nachmittag von Tag 1 in Modul 4.
- Die Ergebnisse werden an Tag 2 in Lab 5.1, Lab 6.1 und Lab 6.2 weiterverwendet.
- Der abschließende Showcase in Lab 8.3 zeigt, welche Artefakte vom Problem bis zum Agenten entstanden sind.

## Praktische Konsequenzen

- Ein gutes Agentenprojekt beginnt nicht mit einem Tool, sondern mit einem belastbaren Problem.
- Jede KI-Ausgabe erhält einen Prüfpunkt: fachlich, technisch, rechtlich oder organisatorisch.
- Prompts, Instruktionen und Skills sind Arbeitsprodukte, keine Chat-Nebenprodukte.
- Unsichere Daten, Berechtigungen und irreversible Aktionen bleiben menschliche Entscheidungen.

Angewendet in Lab 2.3, Modul 4, Lab 5.1, Lab 6.1, Lab 6.2 und Lab 8.3.
