# Lab 8.2 – Übung: Support-Workflow anbinden

**Ändert die Nordwind-Projektbasis?** Ja — der veröffentlichte Agent erhält einen schreibenden Workflow mit Freigabe.

## Ausgangslage

Der Agent ist in Teams getestet. Der Skill `nordwind-it-zugang-beantragen` bereitet Antragsentwürfe vor; der Workflow legt daraus nach Freigabe ein Support-Ticket an und informiert das Support-Team.

## Zielartefakt

Ein Flow-Design und ein Teams-Testnachweis für `Support-Ticket anlegen und benachrichtigen` mit Freigabe vor der finalen Aktion.

## Voraussetzungen und Starterdateien

- SharePoint-Testliste `Support-Tickets` mit Spalten Titel, Kategorie, Priorität, Anfragende Person, Kurzbeschreibung, Status.
- Teams-Kanal für Kursbenachrichtigungen.
- Berechtigung für Agent Flow, SharePoint und Teams-Connector.
- Publish-Rechte für den Agenten nach der Tool-Anbindung.

## Aufgaben

1. Workflow `Support-Ticket anlegen und benachrichtigen` planen: Eingaben, Zielsysteme und Freigabepunkt notieren.
2. Agent Flow mit Trigger **When an agent calls the flow** erstellen.
3. Eingaben für Titel, Kategorie, Priorität, anfragende Person und Kurzbeschreibung definieren.
4. Human-in-the-loop-Freigabe vor die finalen Schreib- und Sendeaktionen setzen.
5. SharePoint-Aktion zum Erstellen des Listeneintrags ergänzen.
6. Teams-Aktion zum Senden einer Kanalbenachrichtigung ergänzen.
7. Antwort an den Agenten konfigurieren und Flow veröffentlichen.
8. Flow als Tool zum Nordwind IT-Helfer hinzufügen und Beschreibung auf Eskalationsfälle begrenzen.
9. Agent erneut veröffentlichen.
10. In Teams eine Zugangs- oder Eskalationsanfrage stellen und dokumentieren: Skill-Entwurf, Tool-Aufruf, Freigabe, Listeneintrag und Nachricht.

## Checkpoint

- Der Flow nutzt den Trigger **When an agent calls the flow**.
- Die Freigabe liegt vor SharePoint- und Teams-Aktion.
- Der Agent wurde nach der Tool-Anbindung erneut veröffentlicht.

## Abschlusskriterien

- Eine Zugangs- oder Eskalationsanfrage erzeugt zuerst einen Entwurf und löst danach kontrolliert den Workflow aus.
- Ticketanlage und Benachrichtigung sind kontrolliert oder als Demo/Fallback dokumentiert.

## Erweiterung

Statusfeld `Neu` automatisch setzen und in der Agentenantwort die Ticketnummer oder Listenelement-ID zurückgeben.

## Fallback

Ohne Schreibrechte: Flow-Designblatt ausfüllen und Trainer-Demo auswerten. Einschränkung: kein eigener SharePoint- oder Teams-Schreibnachweis.
