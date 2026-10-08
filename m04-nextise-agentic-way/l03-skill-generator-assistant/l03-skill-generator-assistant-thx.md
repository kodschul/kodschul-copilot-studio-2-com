# Lab 4.3 – Assistent 3: Skill-Generator

Der Skill-Generator macht aus Architektur und gewähltem Skill zwei Bauartefakte. Dieses Lab erzeugt System-Prompt und eine vollständige `SKILL.md`.

**Leitfragen:**

<details><summary>Was müsste vor produktiver Nutzung des System-Prompts geprüft werden?</summary>
Quellen, Berechtigungen, Eskalationsregeln, Testfälle, Datenschutz und fachliche Freigabe müssen geprüft sein.
</details>

<details><summary>Warum entsteht zusätzlich zur Instruktion eine `SKILL.md`?</summary>
Der System-Prompt steuert den Agenten insgesamt. Die `SKILL.md` kapselt einen wiederholbaren Prozess separat.
</details>

## Zwei Artefakte

| Artefakt | Inhalt | Nutzung |
| --- | --- | --- |
| System-Prompt | Rolle, Ziel, Grenzen, Stil, Eskalation | Agentengrundverhalten |
| `SKILL.md` | Name, Beschreibung, Ablauf, Prüfungen, Ausgabe | wiederverwendbarer Spezialprozess |

## Mindeststruktur einer `SKILL.md`

```markdown
---
name: nordwind-it-zugang-beantragen
description: Deutsche Beschreibung des Skill-Zwecks.
---
# Anweisungen
...
```

| Regel | Grund |
| --- | --- |
| lowercase-hyphen-name | robuste technische Kennung |
| konkrete deutsche Beschreibung | bessere Skill-Auswahl durch den Agenten |
| Markdown-Anweisungen | lesbar, prüfbar, versionierbar |

## Vergleich mit Lab 2.3

Das Instruktionsskelett aus Lab 2.3 bleibt die Basis für Rolle und Grenzen. Assistent 3 ergänzt daraus ein trennbares Skill-Artefakt mit konkretem Ablauf.

> **Merksatz:** Der System-Prompt hält den Agenten auf Kurs; die `SKILL.md` führt eine Teilaufgabe aus.

## Qualitätsprüfung

- Enthält der System-Prompt keine erfundenen Quellen?
- Ist der Skill eng genug für einen wiederholbaren Prozess?
- Gibt es Tests für Normalfall, fehlende Angaben und verbotenen Grenzfall?
- Ist eine menschliche Freigabe bei sensiblen oder irreversiblen Schritten sichtbar?

## Fazit

- Prompt und Skill sind zwei getrennte Artefakte.
- Ein guter Skill hat einen klaren Auslöser und ein prüfbares Ausgabeformat.
- Der Vergleich mit Lab 2.3 zeigt, was aus einer Instruktion wiederverwendbar wird.

Die Übung erzeugt System-Prompt und `SKILL.md` für den gewählten Nordwind-Skill.
