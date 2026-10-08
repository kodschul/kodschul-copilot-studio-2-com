# Lab 8.2 – Lösung: Support-Workflow anbinden

**Ändert die Nordwind-Projektbasis?** Ja — der veröffentlichte Agent erhält einen schreibenden Workflow mit Freigabe.

## Ausgangslage

Der Skill bereitet eine IT-Zugangs- oder Eskalationsanfrage als Entwurf vor. Der Workflow übersetzt den freigegebenen Entwurf in ein Ticket und eine Teams-Benachrichtigung.

## Zielartefakt

Ein vollständiger Nachweis enthält Flow-Design, Tool-Beschreibung, erneutes Publish und Teams-Test.

## Voraussetzungen und Starterdateien

- Liste: `Support-Tickets`.
- Kanal: freigegebener Kurs- oder Support-Kanal.
- Statuswerte im Modell: `Neu`, `In Prüfung`, `Geschlossen`.

## Aufgaben

### 1. Workflow planen

| Feld | Modellantwort |
| --- | --- |
| Name | `Support-Ticket anlegen und benachrichtigen` |
| Eingaben | Titel, Kategorie, Priorität, anfragende Person, Kurzbeschreibung |
| Ziel 1 | SharePoint-Liste `Support-Tickets` |
| Ziel 2 | Teams-Kanalbenachrichtigung |
| Freigabe | vor Listeneintrag und Nachricht |

### 2. Agent Flow erstellen

Trigger: **When an agent calls the flow**.

Grund: Der Agent soll den Flow nur bei passenden Antrags- oder Eskalationsfällen aufrufen.

### 3. Eingaben definieren

| Eingabe | Beispielwert |
| --- | --- |
| `titel` | `VPN-Zugang für neues Notebook beantragen` |
| `kategorie` | `IT-Zugang` |
| `prioritaet` | `mittel` |
| `anfragende_person` | `Kurs-Testperson` |
| `kurzbeschreibung` | `Entwurf aus Skill nordwind-it-zugang-beantragen; fehlende Angaben: Gerätename, Startdatum, Kostenstelle.` |

### 4. Human-in-the-loop-Freigabe setzen

Die Freigabe zeigt mindestens Titel, Kategorie, Zielsysteme und Kurzbeschreibung. Ohne Bestätigung darf keine Schreib- oder Sendeaktion laufen.

### 5. SharePoint-Aktion ergänzen

Aktion: neuen Listeneintrag in `Support-Tickets` erstellen.

| Spalte | Zuordnung |
| --- | --- |
| Titel | `titel` |
| Kategorie | `kategorie` |
| Priorität | `prioritaet` |
| Anfragende Person | `anfragende_person` |
| Kurzbeschreibung | `kurzbeschreibung` |
| Status | `Neu` |

### 6. Teams-Aktion ergänzen

Nachricht im Kanal:

```text
Neues Support-Ticket: {titel}
Kategorie: {kategorie}
Priorität: {prioritaet}
Kurzbeschreibung: {kurzbeschreibung}
Status: Neu
```

### 7. Antwort an den Agenten konfigurieren

Beispielantwort: `Das Support-Ticket wurde nach Freigabe angelegt und das Support-Team wurde benachrichtigt.`

Der Flow wird veröffentlicht, bevor er als Tool erwartet wird.

### 8. Flow als Tool hinzufügen

Tool-Beschreibung:

> Nutze dieses Tool nur, wenn ein vorbereiteter IT-Zugangs-, VPN-, Software- oder Eskalationsentwurf nach menschlicher Freigabe als Ticket in SharePoint angelegt und im Teams-Support-Kanal gemeldet werden soll. Reiche ohne Freigabe nichts ein. Nicht für reine Wissensfragen oder Geräteverfügbarkeit nutzen.

### 9. Agent erneut veröffentlichen

Nach der Tool-Anbindung ist erneutes Publish erforderlich. Ohne erneutes Publish gilt der Teams-Test nicht als Test der aktuellen Agentenversion.

### 10. Zugangs- oder Eskalationsanfrage in Teams testen

**Testanfrage:** „Ich brauche VPN-Zugang für mein neues Notebook.“

**Erwarteter Ablauf:**

1. Skill `nordwind-it-zugang-beantragen` erstellt einen Antragsentwurf und nennt fehlende Angaben.
2. Nach Ergänzung der Pflichtangaben ruft der Agent das Workflow-Tool auf.
3. Freigabe zeigt Ticketdaten vor der Wirkung.
4. Nach Freigabe entsteht ein SharePoint-Listeneintrag.
5. Teams-Kanal erhält Benachrichtigung.
6. Agent meldet die kontrollierte Übergabe zurück.

## Checkpoint

- Trigger, Freigabe und erneutes Publish sind erfüllt.
- Schreib- und Sendeaktionen liegen hinter der Freigabe.
- Der Teams-Test nutzt die veröffentlichte Agentenversion.

## Abschlusskriterien

- Der Workflow-Aufruf ist nach einem vorbereiteten Antrags- oder Eskalationsentwurf nachweisbar.
- Ticket und Benachrichtigung sind kontrolliert entstanden oder als Demo/Fallback dokumentiert.

## Erweiterung

Die Listenelement-ID kann in der Flow-Antwort an den Agenten zurückgegeben werden, etwa: `Ticket #{ID} wurde angelegt.`

## Fallback

Ohne Schreibrechte bleibt die Lösung ein vollständiges Flow-Design und Demo-Protokoll. Live-Schreibzugriffe sind dann vor Kurs im Tenant zu testen.
