# Lab 5.1 – Chat-Agent optimieren

Der Nordwind IT-Helfer wird mit besser getrennten Instruktionen und Wissensquellen nachgeschärft. Das Lab macht sichtbar, ob Antworten aus Wissen, Prompt-Regeln oder Vermutung entstehen.

**Leitfragen:**

<details><summary>Wie zeigt sich, ob eine Antwort aus einer Wissensquelle stammt?</summary>
Die Antwort nennt belegbare Details aus der Datei oder verweist sichtbar auf eine Quelle. Unbelegte Antworten bleiben kritisch, auch wenn sie plausibel klingen.
</details>

<details><summary>Was gehört in Instruktionen und was gehört in Wissen?</summary>
Instruktionen steuern Rolle, Verhalten, Grenzen und Ausgabeform. Wissen liefert Fakten, Richtlinien und Prozessdetails.
</details>

<details><summary>Was hat die Assistenten-Kette gegenüber dem direkten Bau verändert?</summary>
Die Kette trennt Problemklärung, Lösungsentwurf und Prompt-/Skill-Formulierung. Der Chat-Agent erhält dadurch klarere Regeln und testbare Erwartungen.
</details>

## Bausteine im Agent Builder

| Baustein | Zweck | Nordwind-Beispiel |
| --- | --- | --- |
| Instruktionen | Verhalten, Ton, Grenzen, Eskalation | System-Prompt aus Lab 4.3 |
| Wissensquelle | überprüfbare Faktenbasis | IT-Richtlinie und Onboarding-Leitfaden |
| Testprotokoll | Beobachtung statt Bauchgefühl | Fragen aus Lab 3.3 plus zwei neue Fälle |
| Nachschärfung | gezielte Änderung nach Testfehler | Eskalationsregel oder Quellenhinweis präzisieren |

## Wissensquellen im Chat-Agenten

| Quelle | Typische Nutzung | Prüffrage |
| --- | --- | --- |
| Datei | kleine, stabile Richtlinie oder Leitfaden | Wird ein konkreter Dateifakt genannt? |
| SharePoint | geteilte Dokumente und gepflegte Wissensablage | Gelten Berechtigungen und Aktualität? |
| Web | öffentlich erreichbare Inhalte | Ist die Quelle verlässlich und zugelassen? |

Die konkrete Oberfläche des Agent Builders ist tenantabhängig. Bezeichnungen und verfügbare Optionen sind **vor Kursbeginn im Tenant zu prüfen**.

## Instruktion vs. Wissen

| Entscheidung | Gute Praxis | Risiko bei Vermischung |
| --- | --- | --- |
| Verhaltensregel | in Instruktionen schreiben | Regeln verschwinden in langen Dokumenten |
| Fakt aus Richtlinie | als Wissensquelle bereitstellen | Prompt wird schnell veraltet |
| Eskalation | in Instruktionen und Wissen konsistent halten | Agent erfindet Zuständigkeiten |
| Testfrage | gegen erwartete Quelle prüfen | Antwortqualität bleibt subjektiv |

> **Merksatz:** Instruktionen sagen, wie der Agent arbeitet; Wissensquellen sagen, worüber er belastbar antworten darf.

## Nordwind-Szenario

Der einfache Nordwind IT-Helfer aus Lab 3.3 beantwortet bereits Standardfragen. Jetzt ersetzt der System-Prompt aus Lab 4.3 die erste Instruktionsfassung, und die zwei Nordwind-Dokumente werden als Wissen ergänzt.

## Beispiel für Grounding-Prüfung

| Testfrage | Erwartetes belastbares Signal |
| --- | --- |
| „Welches VPN nutzen wir bei Nordwind?“ | Cisco Secure Client, Verbindungsziel und MFA aus der IT-Richtlinie |
| „Was passiert am ersten Arbeitstag?“ | Erstlogin, Passwortwechsel, MFA und Buddy aus dem Onboarding-Leitfaden |
| „Wie hoch ist die Gehaltsbandbreite meiner Position?“ | keine Spekulation, Eskalation an HR |

## Typische Fehlermuster

- Der Agent beantwortet Richtlinienfragen aus allgemeinem Weltwissen statt aus den Dateien.
- Der Prompt enthält Fakten, die eigentlich aus einer Datei gepflegt werden müssten.
- Ein Grenzfall wird freundlich beantwortet, aber nicht eskaliert.
- Eine Quellenanzeige fehlt oder ist im Tenant nicht sichtbar; dann zählt die überprüfbare Antwortsubstanz.

## Fazit

- Der optimierte Chat-Agent entsteht aus klar getrennten Instruktionen, Wissen und Tests.
- Grounding wird über beobachtbare Dateifakten geprüft, nicht über Sprachgefühl.
- Vorher/Nachher-Vergleiche zeigen, ob die Optimierung tatsächlich wirkt.

Die Übung ersetzt Instruktionen, ergänzt Wissen und dokumentiert die Wirkung in einer Testtabelle.
