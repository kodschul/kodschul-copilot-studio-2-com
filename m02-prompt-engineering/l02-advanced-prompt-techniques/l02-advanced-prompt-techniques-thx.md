# Lab 2.2 – Fortgeschrittene Techniken

Dieses Lab vergleicht Prompt-Techniken nach Einsatzkriterium. Der Schwerpunkt liegt auf Supportanfragen, Prüfbarkeit und der Brücke zum Agentic Loop.

**Leitfragen:**

<details><summary>Wann lohnt Few-Shot?</summary>

Few-Shot lohnt, wenn ein gewünschtes Format oder eine Klassifikation durch Beispiele leichter und stabiler gezeigt als beschrieben wird.
</details>

<details><summary>Was unterscheidet ReAct von Chain-of-Thought?</summary>

Chain-of-Thought macht Denk- oder Prüfschritte sichtbar. ReAct verbindet Überlegen mit gezieltem Nachsehen oder Handeln.
</details>

<details><summary>Warum ist ReAct eine Brücke zum Agentic Loop?</summary>

Der Ablauf „denken → handeln → beobachten → entscheiden“ entspricht dem Grundmuster vieler Agentenabläufe.
</details>

## Vergleichstabelle

| Technik | Prinzip | Einsatzkriterium | Risiko |
| --- | --- | --- | --- |
| Zero-Shot | Aufgabe ohne Beispiel stellen | einfache, bekannte Standardfrage | Format und Kategorien schwanken |
| One-Shot | ein Beispiel mitgeben | ein einzelnes Format soll kopiert werden | Beispiel wird übergeneralisiert |
| Few-Shot | mehrere Beispiele mitgeben | Varianten, Tonfall oder Kategorien sollen stabil bleiben | schlechte Beispiele verzerren das Ergebnis |
| Chain-of-Thought | Vorgehen schrittweise sichtbar machen | mehrstufige Analyse oder Begründung erforderlich | sichtbare Schritte können trotzdem falsch sein |
| ReAct | überlegen, Quelle prüfen, Ergebnis bewerten | Antwort hängt von Nachsehen, Tool oder Quelle ab | ohne echte Quelle nur simuliertes Nachsehen |
| Tree-of-Thought | mehrere Lösungswege vergleichen | komplexe Entscheidungen mit Alternativen | hoher Aufwand; im Kurs nur Ausblick |

> **Merksatz:** Few-Shot steuert die Form, Chain-of-Thought steuert den Lösungsweg, ReAct steuert den Wechsel zwischen Denken und Prüfen.

## Nordwind-Supportbeispiel

| Supportfall | Mögliche Technik | Grund |
| --- | --- | --- |
| „Wie richte ich VPN ein?“ | Zero-Shot mit Quelle | klare Standardfrage aus der IT-Richtlinie |
| „Ordne diese fünf Tickets Kategorien zu“ | Few-Shot | Kategorien sollen konsistent bleiben |
| „Ist die Anfrage beantwortbar oder Eskalation?“ | Chain-of-Thought | Kriterien müssen sichtbar geprüft werden |
| „Prüfe Richtlinie und Onboarding-Leitfaden“ | ReAct | mehrere Quellenstellen werden nacheinander geprüft |

## ReAct und Agentic Loop

```text
Gedanke → Handlung/Quelle → Beobachtung → nächster Gedanke → Antwort oder Eskalation
```

| ReAct-Schritt | Agenten-Entsprechung |
| --- | --- |
| Gedanke | Ziel und nächster Prüfschritt |
| Handlung | Wissensquelle, Tool oder Skill nutzen |
| Beobachtung | Ergebnis oder fehlende Information bewerten |
| Antwort | Ergebnis liefern oder eskalieren |

## Grenzen

- Für einfache Ein-Schritt-Fragen erzeugen CoT und ReAct unnötige Länge.
- Sichtbare Zwischenschritte sind prüfbar, aber kein Korrektheitsbeweis.
- Beispiele müssen zur gewünschten Antwortqualität passen.

## Fazit

- Die Technik wird nach Aufgabe gewählt, nicht nach persönlicher Vorliebe.
- Supportfragen profitieren besonders von Quellenbindung, Beispielen und Eskalationskriterien.
- ReAct bereitet auf agentische Abläufe mit Tool- und Quellenprüfung vor.

Die Übung vergleicht Zero-Shot mit Few-Shot und Chain-of-Thought an einer Nordwind-Supportanfrage.
