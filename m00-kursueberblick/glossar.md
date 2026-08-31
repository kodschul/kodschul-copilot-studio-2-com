# Glossar: KI-Agenten mit Microsoft Copilot Studio & Power Automate (EFG)

Alle Begriffe in alphabetischer Reihenfolge. Kompakte Fassung siehe auch [handout.md](../handout.md).

---

**Agent**
Ein KI-System, das eine Aufgabe versteht, selbst entscheidet, welche Schritte/Werkzeuge nötig sind, und
diese ausführt — im Unterschied zum Chatbot handelt ein Agent, statt nur zu antworten.

**Aktion (Flow-Aktion)**
Ein Schritt in Power Automate, der etwas ausführt, z. B. "Zeile in Excel hinzufügen" oder "E-Mail senden".

**ChatGPT**
Eigenständiges Produkt von OpenAI, sehr breit einsetzbar, aber ohne besondere Anbindung an Firmendaten.

**Claude**
Eigenständiges Produkt von Anthropic, stark bei Text/Code, ebenfalls ohne Standard-Anbindung an M365.

**Connector**
Verbindung zwischen Power Automate und einem System/einer App (z. B. SharePoint-, Excel-, Outlook-Connector).

**Copilot**
Produktfamilie von Microsoft, tief in M365 integriert (Outlook, Teams, SharePoint).

**Copilot Studio**
Low-Code-Plattform von Microsoft zum Erstellen von Agenten aus Instruktionen, Wissen, Tools/Skills und Themen.

**Flow**
Ein in Power Automate erstellter automatisierter Ablauf aus Trigger und Aktionen.

**Instruktionen**
Der System-Prompt eines Agenten — fest hinterlegt, begleitet jede Anfrage (Rolle, Sprache, Ausgabeformat).

**Knowledge (Wissen)**
Dateien, SharePoint-Seiten oder Webseiten, die ein Agent als Wissensbasis nutzt, um nicht zu halluzinieren.

**Modell**
Die KI-"Engine" im Hintergrund (z. B. GPT, Claude, Gemini) — abzugrenzen vom Produkt, in dem sie genutzt wird.

**Power Automate (Cloud)**
Automatisierungsplattform mit Trigger → Aktion über Connectors.

**Power Automate Desktop**
Variante für Alt-/Desktop-Anwendungen ohne Cloud-Connector, simuliert Mausklicks/Tastatureingaben.

**Prompt**
Die Anweisung an den Agenten — Nutzer-Prompt (einzelne Anfrage) oder Instruktionen (fest hinterlegter
System-Prompt).

**Skill / Tool**
Eine konkrete Fähigkeit, die ein Agent bei Bedarf aufruft (z. B. „Datei lesen", „Flow in Power Automate
auslösen"). Der Agent entscheidet selbst, wann er welches Tool braucht.

**Testfenster**
Bereich in Copilot Studio, in dem der Agent direkt während der Konfiguration ausprobiert werden kann.

**Trigger**
Das Ereignis, das einen Flow startet (z. B. "neue Datei in SharePoint" oder "von Copilot Studio aufgerufen").
