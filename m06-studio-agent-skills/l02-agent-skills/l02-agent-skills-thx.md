# Lab 6.2 – Skills hinzufügen

Skills kapseln wiederverwendbares Agentenverhalten als eigenes Paket aus Beschreibung, Anweisungen und optionalen Ressourcen. Dieses Lab ergänzt den Nordwind Studio-Agenten um erste Skills und testet deren Auslösung.

**Leitfragen:**

<details><summary>Woran entscheidet der Agent, einen Skill zu laden?</summary>
Vor allem an der Skill-Beschreibung und daran, ob die Anfrage zu Zweck, Grenzen und Ausgabeformat passt.
</details>

<details><summary>Warum sollten Skills klein bleiben?</summary>
Kleine Skills triggern zuverlässiger, lassen sich einzeln testen und konkurrieren weniger mit globalen Instructions.
</details>

<details><summary>Wann ist ein Skill besser als eine weitere Instruktion?</summary>
Wenn ein wiederholbarer Teilauftrag eigene Schritte, Sonderfälle oder ein festes Ausgabeformat braucht.
</details>

## Skill-Anatomie

| Baustein | Aufgabe | Gute Ausprägung |
| --- | --- | --- |
| Name | technische Kennung | klein, eindeutig, nur Kleinbuchstaben, Zahlen und Bindestriche |
| Description | Aktivierungssignal | Anlass, Zweck, Grenze und Zielausgabe klar genannt |
| Markdown-Anweisungen | Arbeitslogik | Schritte, Format, Sonderfälle und erlaubte Quellen |
| Ressourcen | optionaler Zusatzkontext | nur ergänzen, wenn wirklich gebraucht |

## Abgrenzung zu anderen Bausteinen

| Baustein | Rolle im Agenten | Nordwind-Beispiel |
| --- | --- | --- |
| Instructions | allgemeines Verhalten | keine Vermutungen, Sonderfälle eskalieren |
| Knowledge | Faktenbasis | IT-Richtlinie, Onboarding-Leitfaden |
| Tools | externe Aktion | späterer Workflow oder Konnektor |
| Skills | wiederverwendbarer Teilauftrag | VPN erklären, Checkliste erstellen, Eskalation vorbereiten |

## Drei Erstellungswege

| Weg | Einsatz im Lab | Nutzen |
| --- | --- | --- |
| Upload a Skill | `SKILL.md` aus Lab 4.3 hochladen | vorhandenes Ergebnis weiterverwenden |
| Generate with AI | zweiten Skill natürlichsprachlich beschreiben | schnelle erste Fassung plus Rückfragen |
| Create from blank | optionalen dritten Skill manuell anlegen | volle Kontrolle über Beschreibung und Schritte |

## Progressive Disclosure

Der GitHub-Copilot-Harness lädt Skill-Kontext nur bei Bedarf. Dadurch bleiben globale Instructions schlank, während wiederkehrende Teilaufgaben detaillierter beschrieben werden können.

> **Merksatz:** Die Skill-Beschreibung ist der Schalter; der Skill-Body ist erst nach dem Auslösen wirksam.

## Trigger-Test

| Testtyp | Zweck | Beispiel |
| --- | --- | --- |
| Standardfall | Skill soll auslösen | „VPN auf dem Firmenlaptop einrichten“ |
| Variante | andere Formulierung soll ebenfalls passen | „Remote ins Nordwind-Netz verbinden“ |
| Nicht-Auslöser | Skill soll aus bleiben | „Wie hoch ist mein Gehalt?“ |

## Häufige Fehlmuster

- Beschreibung ist zu breit und triggert bei jeder Supportfrage.
- Beschreibung nennt nur ein Format, aber keinen fachlichen Anlass.
- Skill enthält zu viele Aufgaben und konkurriert mit anderen Skills.
- Nicht-Auslöser fehlen, daher greift der Skill bei Grenzfällen.

## Fazit

- Skills modularisieren wiederkehrende Teilaufgaben ohne globale Instructions aufzublähen.
- Gute Beschreibungen enthalten Anlass, Zweck, Grenze und Ergebnis.
- Preview-Tests mit Standardfall, Variante und Nicht-Auslöser machen Triggerqualität sichtbar.

Die Übung lädt einen vorhandenen Skill hoch, erzeugt einen zweiten Skill mit KI und schärft Beschreibungen anhand von Preview-Beobachtungen.
