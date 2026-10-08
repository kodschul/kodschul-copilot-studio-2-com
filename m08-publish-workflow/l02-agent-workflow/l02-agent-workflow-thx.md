# Lab 8.2: Workflow anbinden

Ein Workflow macht aus einer passenden Eskalation einen kontrollierten Ablauf. Dieses Lab bindet einen SharePoint- und Teams-Workflow als Tool an den veröffentlichten Agenten.

**Leitfragen:**

<details><summary>Woran erkennt der Agent, wann er den Workflow aufruft?</summary>
Die Tool-Beschreibung grenzt Zweck und Nicht-Einsatzfälle ab. Der Agent entscheidet anhand Anfrage und Beschreibung.</details>

<details><summary>Wo gehört die menschliche Freigabe hin?</summary>
Vor die finale Schreib- oder Sendaktion. Danach wäre die Kontrolle nur noch Nachprüfung.</details>

<details><summary>Warum erneut veröffentlichen?</summary>
Ein neu angebundenes Tool ist für Teams-Nutzende erst nach erneutem Publish und neuer Session zuverlässig verfügbar.</details>

## Kernbegriffe

| Begriff | Bedeutung |
| --- | --- |
| Workflow | deterministischer Ablauf aus Trigger und Aktionen |
| Agent flow | Flow, der als Tool im Agenten nutzbar sein kann |
| Trigger | Ereignis, das den Workflow startet |
| When an agent calls the flow | Trigger, mit dem ein Flow als Agent-Tool genutzt werden kann |
| Human in the loop | menschliche Rückfrage oder Freigabe im Ablauf |
| Respond to the agent | Antwortschritt, der Ergebnis an den Agenten zurückgibt |

## Automatisierung, Workflow und Agent

| Baustein | Rolle im Kurs |
| --- | --- |
| Agent | bewertet Anfrage und entscheidet, ob Antrag oder Eskalation nötig ist |
| Skill | bereitet den Antrags- oder Eskalationsentwurf vor, reicht ihn aber nicht ein |
| Workflow | erstellt nach Freigabe das Ticket und sendet die Benachrichtigung |
| Mensch | prüft vor der finalen Aktion |
| Power Automate | Plattformkontext für Cloud-Flows und Connector-Aktionen |

## Verifizierter Rahmen

| Fakt | Bedeutung |
| --- | --- |
| Workflow = Trigger + mindestens eine Aktion | Basismodell für den Ablauf |
| Aktionen können Connectoren und Human-in-the-loop enthalten | SharePoint, Teams und Freigabe sind plausibel |
| `When an agent calls the flow` macht Workflow als Tool nutzbar | Kurs-Trigger für die Agent-Anbindung |
| Flow als Tool braucht Antwort an Agent und Veröffentlichung | vor Kurs im Tenant prüfen |

> **Merksatz:** Der Skill formuliert den Entwurf; der Workflow erzeugt nach Freigabe die Wirkung.

## Quellen

- Quelle: Microsoft Learn, **Workflows overview**, abgerufen am 07.10.2026.
- Quelle: Microsoft Learn, **Add an agent flow as a tool to an agent**, abgerufen am 07.10.2026.

## Fazit

- Workflows sind der deterministische Teil im agentischen Gesamtbild.
- Schreibende Aktionen brauchen eine Freigabe vor der Wirkung.
- Nach Tool-Änderungen ist erneutes Publish für Teams Pflicht.

Die Übung baut `Support-Ticket anlegen und benachrichtigen`, ergänzt eine Freigabe und löst die Eskalation in Teams aus.
