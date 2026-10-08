# Lab 2.4 – Lösung: HITL-Gliederung für den Support-Agenten

## Ausgangslage

Die Lösung zeigt ein mögliches Designgerüst für den Nordwind IT-Helfer. Das Gerüst ergänzt die Instruktion aus Lab 2.3, ersetzt sie aber nicht.

## Zielartefakt

Eine Notiz `hitl-agent-outline.md` mit Vision, gekürzter Gliederung, Kerninhalten und Belegstatus.

## Voraussetzungen

Die Belegstatus beziehen sich auf die Nordwind-IT-Richtlinie und den Nordwind-Onboarding-Leitfaden.

## Aufgaben

### 1. Vision ohne Copilot formulieren

Muster:

```text
Der Nordwind IT-Helfer beantwortet interne Standardfragen zu IT und Onboarding für Mitarbeitende und neue Mitarbeitende. Ziel ist schnelle Orientierung mit klarer Eskalation bei Ausnahmen, Sonderrechten und HR-Themen.
```

### 2. Alternativformulierungen auswählen

Mögliche Auswahlbegründung: Die gewählte Fassung nennt Zielgruppe, Themenrahmen und Eskalation. Eine rein werbliche Formulierung wäre weniger prüfbar.

### 3. Gliederung vorschlagen lassen

Möglicher Rohvorschlag:

1. Zielgruppe
2. Typische IT-Fragen
3. Onboarding-Fragen
4. VPN und MFA
5. Softwarebeantragung
6. Geräte und private Nutzung
7. HR-Fragen
8. Sonderberechtigungen
9. Eskalation
10. Antwortformat
11. Qualitätskriterien
12. Grenzen

### 4. Gliederung kürzen

| Entscheidung | Begründung |
| --- | --- |
| VPN/MFA in „Typische IT-Fragen“ zusammengeführt | redundant |
| Softwarebeantragung in „Typische IT-Fragen“ integriert | Detail |
| HR-Fragen unter „Grenzen“ verschoben | nicht zuständig |
| Sonderberechtigungen unter „Eskalation“ verschoben | Ausnahme |
| Antwortformat mit Qualitätskriterien kombiniert | eng verwandt |

Gekürzte Gliederung:

1. Zielgruppe
2. Abgedeckte Fragen
3. Wissensquellen
4. Grenzen
5. Eskalation
6. Antwort- und Qualitätskriterien

### 5. Kernaussagen formulieren

| Punkt | Kernaussage |
| --- | --- |
| Zielgruppe | Mitarbeitende und neue Mitarbeitende erhalten Orientierung zu IT- und Onboarding-Standardfragen. |
| Abgedeckte Fragen | VPN, MFA, Firmengeräte, Standardsoftware, Ticket-Portal und erste 30 Tage sind Kernfragen. |
| Wissensquellen | IT-Richtlinie und Onboarding-Leitfaden sind die maßgeblichen Quellen. |
| Grenzen | Vertrags-, Gehalts-, Sonderberechtigungs- und rechtliche Fragen werden nicht beantwortet. |
| Eskalation | Nicht abgedeckte oder individuelle Fälle gehen an IT-Support oder HR. |
| Antwort- und Qualitätskriterien | Antworten bleiben kurz, quellengebunden und nennen bei Bedarf den Kontaktweg. |

### 6. Belegstatus markieren

| Punkt | Belegstatus |
| --- | --- |
| Zielgruppe | Kurskontext, nicht direkt Quelle |
| Abgedeckte Fragen | beide Quellen |
| Wissensquellen | beide Quellen |
| Grenzen | beide Quellen, HR-Grenze aus Onboarding-Leitfaden |
| Eskalation | beide Quellen |
| Antwort- und Qualitätskriterien | Instruktionsentscheidung, offen für Lab 3.3 |

### 7. Ergebnis sichern

Musterinhalt für `hitl-agent-outline.md`:

```text
# HITL-Gliederung Nordwind IT-Helfer

Vision: Der Nordwind IT-Helfer beantwortet interne Standardfragen zu IT und Onboarding für Mitarbeitende und neue Mitarbeitende. Ziel ist schnelle Orientierung mit klarer Eskalation bei Ausnahmen, Sonderrechten und HR-Themen.

1. Zielgruppe – Mitarbeitende und neue Mitarbeitende; Beleg: Kurskontext.
2. Abgedeckte Fragen – VPN, MFA, Firmengeräte, Standardsoftware, Ticket-Portal, erste 30 Tage; Beleg: beide Quellen.
3. Wissensquellen – IT-Richtlinie und Onboarding-Leitfaden; Beleg: beide Quellen.
4. Grenzen – keine Vertrags-, Gehalts-, Sonderberechtigungs- oder Rechtsfragen; Beleg: beide Quellen.
5. Eskalation – IT-Support oder HR je nach Fall; Beleg: beide Quellen.
6. Antwortqualität – kurz, quellengebunden, mit Kontaktweg; Beleg: Instruktionsentscheidung.
```

## Checkpoint

- Die Vision ist vor Copilot formuliert.
- Mehrere Punkte wurden gestrichen oder zusammengeführt.
- Jede Kernaussage hat einen Belegstatus.

## Abschlusskriterien

- Zielgruppe, Fragen, Grenzen und Eskalation sind enthalten.
- Offene oder konzeptionelle Punkte sind als solche markiert.
- Die Gliederung lässt sich mit Lab 2.3 abgleichen.

## Erweiterung

Mögliche Risiken:

| Risiko | Einordnung |
| --- | --- |
| Quellen veralten | vor Kurs und vor Veröffentlichung prüfen |
| Agent beantwortet HR-Fragen | Grenze und Eskalation testen |
| Sonderberechtigungen werden zugesagt | negative Testfälle aufnehmen |

## Fallback

Eine von Hand erstellte Gliederung ist gültig, wenn sie dieselben Entscheidungen sichtbar macht. Fehlende KI-Alternativen sind kein fachlicher Mangel.
