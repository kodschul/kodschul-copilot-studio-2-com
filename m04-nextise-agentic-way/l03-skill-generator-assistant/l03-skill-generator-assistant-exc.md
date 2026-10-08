# Lab 4.3 – Übung: System-Prompt und SKILL.md erzeugen

## Ausgangslage

Das Architekturpaket aus Lab 4.2 enthält den gewählten Skill. Jetzt entstehen ein System-Prompt und eine uploadfähige `SKILL.md`.

## Zielartefakt

Ein System-Prompt und eine vollständige `SKILL.md` für einen Skill entstehen. Beide Artefakte werden für Lab 5.1 und Lab 6.2 gespeichert.

## Voraussetzungen und Starter

- Übergabepaket aus Lab 4.2
- Assistent-3-Prompt aus `../01-assistenten-prompts.md`
- Instruktionsskelett aus `../../m02-prompt-engineering/l03-agent-instructions/` oder lokale Kopie
- Notizbereich für Prompt, Skill und Vergleich

## Aufgaben

1. Einen neuen Assistenten oder Chat mit dem Prompt „Assistent 3 – Skill-Generator“ anlegen.
2. Übergabepaket aus Lab 4.2 einfügen und genau einen Skill nennen.
3. System-Prompt erzeugen lassen.
4. Eine vollständige `SKILL.md` erzeugen lassen: `name`, `description`, Markdown-Anweisungen.
5. System-Prompt mit dem eigenen Skelett aus Lab 2.3 vergleichen: Rolle, Scope, Quellenregel, Eskalation, Stil.
6. Eine Testliste ergänzen: Normalfall, fehlende Angaben, Grenzfall außerhalb des Zwecks.
7. System-Prompt und `SKILL.md` so speichern, dass beide in Lab 5.1 und Lab 6.2 auffindbar sind.

## Checkpoint

- System-Prompt und `SKILL.md` sind getrennt.
- Skill-Name erfüllt lowercase-hyphen.
- Beschreibung ist Deutsch und konkret.
- Mindestens drei Tests sind dokumentiert.

## Abschlusskriterien

- Beide Artefakte sind vollständig kopierbar.
- Der Vergleich mit Lab 2.3 nennt mindestens eine Verbesserung und eine offene Prüfung.

## Erweiterung

Den Skill-Namen gegen eine zu vage Alternative vergleichen und begründen, warum der präzisere Name besser auslösbar ist.

## Fallback

Ohne eigenen Assistenten wird der Prompt in einem normalen Chat genutzt. Die Einschränkung: keine persistente Agentenrolle und kein realer Skill-Upload.
