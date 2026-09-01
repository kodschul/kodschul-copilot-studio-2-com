# FAQ: KI-Agenten mit Microsoft Copilot Studio & Power Automate (EFG)

Häufig gestellte Fragen aus Teilnehmenden-Perspektive und vom Trainer.

---

## Zugang und Voraussetzungen

**Welche Lizenzen brauchen wir für das Training?**
Mit M365 Business ist die Basisnutzung von Copilot Studio und Power Automate bereits enthalten
(siehe [00-eckdaten.md](../00-eckdaten.md)). Bestimmte Premium-Connectors oder hohe Nutzungsvolumen
können Zusatzkosten auslösen — im Zweifel vor Ort/mit Microsoft-Partner klären.

**Muss ich programmieren können?**
Nein. Alle Übungen sind Low-Code über die Copilot-Studio- und Power-Automate-Oberflächen.

---

## Solarcomputer-Anbindung

**Gibt es einen direkten Connector zu Solarcomputer?**
Nicht bestätigt (offener Punkt, siehe [00-eckdaten.md](../00-eckdaten.md) und M08). Falls nein:
Zwischenschritt über Excel/SharePoint oder Power Automate Desktop (Mausklick-/Tastatur-Simulation).

**Was, wenn wir während der Schulung keinen Testzugang zu Solarcomputer haben?**
Fallback: Power-Automate-Desktop-Prinzip an einer Ersatz-Desktop-Anwendung zeigen (z. B. Notepad/Rechner),
das Vorgehen bleibt identisch — siehe Fallback-Optionen in [trainer-guide.md](../trainer-guide.md).

---

## Copilot Studio

**Was ist der Unterschied zwischen einem Agenten und einem klassischen Chatbot?**
Ein Chatbot antwortet nur auf Basis von Text. Ein Agent kann zusätzlich Tools/Skills aufrufen und damit
handeln (z. B. einen Plan einlesen und die Werte automatisiert weitergeben) — siehe M02.

**Warum liefert unser Extraktions-Agent manchmal falsche Werte?**
Meistens einer von drei Gründen:

1. Die Planqualität ist schlecht (Scan, Handschrift, uneinheitliches Layout).
2. Die Instruktionen sind zu ungenau formuliert (Ausgabeformat nicht klar beschrieben).
3. Der Plan enthält Sonderfälle, die im Beispiel nicht vorkamen (z. B. fehlende Raumbezeichnung).

**PDF oder DXF — was ist zuverlässiger?**
DXF liefert tendenziell zuverlässigere Ergebnisse, da die Daten strukturiert vorliegen (LINE-/TEXT-
Entitäten). PDF ist aber der bei EFG häufigste, oft einzig verfügbare Fall (siehe M07).

---

## Nach der Schulung

**Was ist der empfohlene nächste Schritt?**
Ein Pilotprojekt mit echten EFG-Testdaten, plus Klärung der Solarcomputer-Anbindung mit IT/Microsoft-
Partner (siehe M10).
