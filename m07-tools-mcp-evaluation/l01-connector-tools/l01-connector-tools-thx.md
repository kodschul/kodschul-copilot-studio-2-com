# Lab 7.1: Konnektoren als Tools

Ein Tool erweitert den Nordwind IT-Helfer um eine klar beschriebene Fähigkeit. Dieses Lab zeigt einen lesenden Microsoft-365-Konnektor als kontrollierte Tool-Erweiterung.

**Leitfragen:**

<details><summary>Warum entscheidet die Tool-Beschreibung über den Aufruf?</summary>
Die Orchestrierung nutzt Name, Zweck und Beschreibung, um ein passendes Tool auszuwählen. Unklare Beschreibungen erzeugen Fehlaufrufe.</details>

<details><summary>Was ändert sich am Risiko, sobald ein Tool schreiben darf?</summary>
Ein schreibendes Tool verändert Daten oder löst Folgeprozesse aus. Deshalb braucht es strengere Freigabe, Eingrenzung und meist menschliche Bestätigung.</details>

<details><summary>Welche Rolle spielt die Verbindung?</summary>
Die Verbindung bestimmt, mit welchen Berechtigungen der Connector auf Daten zugreift. Tenant-, DLP- und Zugriffspolitik bleiben maßgeblich.</details>

## Kernbegriffe

| Begriff | Bedeutung |
| --- | --- |
| Tool | Fähigkeit des Agenten, ein externes System zu nutzen oder eine Aktion auszuführen |
| Connector | Power-Platform-Anbindung an Microsoft-365-, Drittanbieter- oder eigene Dienste |
| Read-only | Tool liest Daten, verändert aber keine Einträge |
| Write | Tool erzeugt, ändert, teilt oder löscht Daten |
| Connection | Authentifizierte Verbindung zum Zielsystem |
| DLP-Richtlinie | Organisationsregel, die Connectoren und Datenwege erlauben oder blockieren kann |

## Tool-Typen in Copilot Studio

| Mechanismus | Typischer Zweck | Kursbeispiel |
| --- | --- | --- |
| Connector | Dienst anbinden, Daten lesen oder Aktionen ausführen | SharePoint `Get items` auf Liste `IT-Geräte` |
| REST API / Custom connector | eigene API kontrolliert verfügbar machen | nur als Ausblick |
| Agent flow / Workflow | festen Ablauf als Tool anbieten | Lab 8.2 |
| MCP | Tool- oder Resource-Katalog eines MCP-Servers nutzen | Lab 7.2 |
| Prompt | einmalige Modellaufgabe als Tool kapseln | optional |

## Warum zuerst lesend?

| Entscheidung | Grund |
| --- | --- |
| Lesender Connector | sichtbarer Nutzen bei geringerer Nebenwirkung |
| Kleine Testliste | reproduzierbares Ergebnis ohne Produktivdaten |
| Klare Tool-Beschreibung | Agent ruft das Tool nur für passende Gerätefragen auf |
| Preview-Beobachtung | Tool-Aufruf wird vor Veröffentlichung geprüft |

> **Merksatz:** Jedes Tool ist eine Fähigkeit und eine Zugriffsfläche zugleich.

## Nordwind-Szenario

Der IT-Helfer beantwortet Wissensfragen aus Richtlinie und Onboarding-Leitfaden. Für Geräteverfügbarkeit soll er zusätzlich die freigegebene SharePoint-Liste `IT-Geräte` lesen.

## Verifizierter Rahmen

- Microsoft Learn nennt Connectoren, Agent flows, REST APIs und MCP als Mechanismen für Tools.
- Der SharePoint-Connector ist für Copilot Studio gelistet und enthält die Aktion `Get items`.
- Der genaue Klickpfad und die konkrete Freigabe im GitHub-Copilot-Harness bleiben vor Kurs im Tenant zu prüfen.

## Quellen

- Quelle: Microsoft Learn, **Add tools to custom agents**, abgerufen am 07.10.2026.
- Quelle: Microsoft Learn, **SharePoint - Connectors**, abgerufen am 07.10.2026.

## Fazit

- Tools erweitern den Agenten über Wissen hinaus in Richtung Handlung oder Systemzugriff.
- Read-only ist der sichere Startpunkt für erste Connector-Labs.
- Name, Beschreibung, Verbindung und DLP-Regeln entscheiden über Nutzbarkeit und Risiko.

Die Übung ergänzt einen freigegebenen lesenden Connector und beobachtet den Tool-Aufruf in Preview.
