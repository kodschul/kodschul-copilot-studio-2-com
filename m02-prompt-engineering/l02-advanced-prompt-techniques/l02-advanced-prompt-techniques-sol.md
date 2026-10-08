# Lab 2.2 – Lösung: Supportanfrage mit Techniken vergleichen

## Ausgangslage

Die Lösung nutzt die Nordwind-IT-Richtlinie. Live-Ergebnisse können im Wortlaut abweichen, müssen aber die Richtliniengrenze erhalten.

## Zielartefakt

Eine Vergleichstabelle mit Zero-Shot, Few-Shot/Chain-of-Thought, Qualitätsbewertung und Entscheidung.

## Voraussetzungen

Die relevante Richtlinienpassage lautet sinngemäß: Private Geräte dürfen nur über mobile Outlook-/Teams-App mit App-Schutzrichtlinie genutzt werden, nicht über VPN.

## Aufgaben

### 1. Zero-Shot-Prompt formulieren

```text
Eine Person bei Nordwind fragt: Darf ein privates Notebook per VPN genutzt werden, und was ist stattdessen möglich? Antworte kurz für den internen IT-Support.
```

### 2. Ergebnis speichern und prüfen

Erwarteter Befund:

| Kriterium | Typische Zero-Shot-Beobachtung |
| --- | --- |
| Quelle | häufig nicht explizit genannt |
| Grenze | private VPN-Nutzung kann unklar formuliert sein |
| Eskalation | oft fehlend |
| Ton | meist brauchbar, aber generisch |

### 3. Few-Shot- oder Chain-of-Thought-Variante formulieren

Muster mit Chain-of-Thought-Prüfschritten:

```text
Rolle: Interner IT-Support für Nordwind Consulting.
Grundlage: Nordwind-IT-Richtlinie.
Aufgabe: Beantworte die Frage zu privatem Notebook und VPN.
Gehe sichtbar in drei Prüfschritten vor:
1. Welche Regel gilt für private Geräte?
2. Welche erlaubte Alternative nennt die Richtlinie?
3. Muss eskaliert werden oder reicht eine Standardantwort?
Antworte danach in maximal vier Stichpunkten.
```

Alternative Few-Shot-Beispiele:

```text
Beispiel 1: Frage nach VPN-Zertifikat → Antwort: Standardregel nennen, bei Ablauf an IT-Support verweisen.
Beispiel 2: Frage nach Gehaltsdetails → Antwort: nicht beantworten, an HR eskalieren.
Neue Frage: Darf ein privates Notebook per VPN genutzt werden, und was ist stattdessen möglich?
```

### 4. Ergebnisse vergleichen

| Kriterium | Zero-Shot | Few-Shot/Chain-of-Thought |
| --- | --- | --- |
| Quelle | schwach sichtbar | Richtlinie wird als Grundlage genannt |
| Grenze | kann weich bleiben | private Geräte nicht per VPN, keine Sonderfreigabe |
| Eskalation | oft fehlend | bei Ausnahme oder Sonderberechtigung an IT-Support |
| Nutzbarkeit | schnell, aber prüfbedürftig | besser für Supportstandard geeignet |

### 5. ReAct-Variante skizzieren

```text
Gedanke: Für private Geräte muss zuerst die Geräte- und Passwortrichtlinie geprüft werden.
Handlung: Abschnitt „Geräte- und Passwortrichtlinie“ lesen.
Beobachtung: Private Geräte nur über mobile Outlook-/Teams-App mit App-Schutzrichtlinie, nicht über VPN.
Gedanke: Die Anfrage kann als Standardregel beantwortet werden; Sonderfreigabe wäre Eskalation.
Antwort: Regel, erlaubte Alternative und Eskalationsweg nennen.
```

### 6. Entscheidung begründen

Musterentscheidung: Für diese Anfrage passt Chain-of-Thought mit Quellenbindung am besten, weil die Antwort eine Richtliniengrenze und eine Eskalationsentscheidung sichtbar prüfen muss. Few-Shot ist nützlich, wenn viele Supportantworten im gleichen Format entstehen sollen.

## Checkpoint

- Zwei Ergebnisse sind vorhanden und einer Technik zugeordnet.
- Die Vergleichstabelle bewertet Quelle, Grenze, Eskalation und Nutzbarkeit.
- Die Entscheidung nutzt ein Kriterium, nicht Geschmack.

## Abschlusskriterien

- Die Lösung erlaubt keinen VPN-Zugang für private Notebooks.
- Die zulässige Alternative sind mobile Outlook-/Teams-Apps mit App-Schutzrichtlinie.
- Sonderfälle werden an IT-Support oder passende Stelle eskaliert.

## Erweiterung

Für zusätzliche Software passt ein wiederverwendbarer Supportprompt gut:

| Punkt | Erwartung |
| --- | --- |
| Regel | zusätzliche Fachsoftware über IT-Ticket-Portal beantragen |
| Entscheidung | nicht durch den Agenten zusagen |
| Stabilität | Few-Shot kann Antwortformat und Eskalationssatz stabilisieren |

## Fallback

Die vorhergesagten Unterschiede sind ausreichend, wenn die Richtliniengrenze korrekt erkannt wird. Ohne Live-Test ist keine Aussage zur tatsächlichen Modellstabilität möglich.
