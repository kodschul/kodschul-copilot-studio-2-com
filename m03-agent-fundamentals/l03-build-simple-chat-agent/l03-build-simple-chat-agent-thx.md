# Lab 3.3 – Ersten Chat-Agenten bauen

Der erste Nordwind IT-Helfer entsteht im Copilot-Chat-Agent-Builder ohne Wissensquelle. Dieses Lab erzeugt eine Baseline und macht die Grenzen fehlenden Firmenwissens sichtbar.

**Leitfragen:**

<details><summary>Welche drei Angaben braucht ein Agent mindestens?</summary>
Name, Beschreibung und Instruktionen reichen für einen ersten Test. Für belastbare Fachantworten kommt später Wissen hinzu.
</details>

<details><summary>Woran erkennt man fehlendes Firmenwissen?</summary>
Antworten bleiben allgemein, raten Details oder eskalieren nicht sauber. Ein Testlog macht diese Schwächen sichtbar.
</details>

<details><summary>Was unterscheidet Beschreiben und Konfigurieren?</summary>
Beschreiben startet natürlichsprachlich; Konfigurieren macht Felder, Regeln und Starter-Prompts explizit sichtbar.
</details>

## Bausteine im Agent Builder

| Feld | Zweck für den Nordwind IT-Helfer |
| --- | --- |
| Name | sichtbarer Agentenname, z. B. „Nordwind IT-Helfer“ |
| Beschreibung | kurze Erwartung für Nutzende und Agentenauswahl |
| Instruktionen | Rolle, Umfang, Stil, Grenzen, Eskalation |
| Starter-Prompts | typische Einstiegsfragen für den Test |
| Wissen | in diesem Lab bewusst leer |

## Beschreiben vs. Konfigurieren

| Arbeitsweise | Vorteil | Risiko |
| --- | --- | --- |
| Beschreiben | schneller Start aus einer natürlichsprachlichen Idee | wichtige Grenzen bleiben implizit |
| Konfigurieren | klare Felder und prüfbare Regeln | etwas mehr Sorgfalt beim Ausfüllen |
| Kombination | Idee grob beschreiben, dann Felder prüfen | nur tragfähig, wenn Tests folgen |

## Instruktionsskelett aus Lab 2.3

Das Skelett aus `../../m02-prompt-engineering/l03-agent-instructions/` liefert Rolle, Ziel, Quellenregel, Eskalation und Antwortstil. Falls der parallele Stand noch nicht vorliegt, reicht eine knappe Fassung dieser Felder.

## Testlog als Baseline

| Testfrage | Erwartung ohne Wissen | Beobachtung | Schwäche | Nacharbeit |
| --- | --- | --- | --- | --- |
| VPN-Frage | keine belegte Nordwind-Antwort | offen | mögliches Raten | Wissen ergänzen |
| Erster Arbeitstag | keine belegte Nordwind-Antwort | offen | allgemeines Onboarding | Wissen ergänzen |
| Gehaltsfrage | Eskalation an HR | offen | Grenzfallprüfung | Instruktion schärfen |

> **Merksatz:** Ein Agent ohne Wissensquelle ist ein Verhaltenstest, kein verlässlicher Fachagent.

## Typische Schwächen

- Firmennamen, Tools oder Fristen können erfunden wirken.
- Allgemeinwissen ersetzt keine Nordwind-Quelle.
- Grenzfälle werden nur sauber behandelt, wenn die Instruktion explizit ist.

## Fazit

- Der erste Chat-Agent prüft Rolle, Stil und Grenzen.
- Fehlendes Wissen wird absichtlich sichtbar und im Testlog dokumentiert.
- Die Baseline aus Agent und Testlog wird in späteren Labs verbessert.

Die Übung baut den Nordwind IT-Helfer ohne Wissensquelle und dokumentiert drei Testläufe.
