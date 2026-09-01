# M09 Theorie: Use Case 2 — Aufmaßprüfung

> Lesetext für die Teilnehmenden und Showcase-Vorlage für den Trainer. Trainer-Hinweise stehen
> gesammelt im Abschnitt "Trainer-Showcase".

## Lernziel

Nach diesem Modul könnt ihr ein Agenten-Konzept für einen Soll/Ist-Abgleich skizzieren und die
Machbarkeit realistisch einschätzen.

## Dauer

Tag 2 · 15:00–16:15 · 75 Minuten

## Ausgangslage

Eine Massenaufstellung (Liste mit erwarteten Mengen) muss gegen Pläne (meist PDF, teils DXF) geprüft
werden. Der Unterschied zu Use Case 1: hier geht es um **Abgleich/Prüfung**, nicht nur um Extraktion.

## Konzeptionelle Skizze eines Prüf-Agenten

In Kleingruppen wird ein Agent-Konzept skizziert (kein vollständiger Build, da die Zeit begrenzt ist).
Leitfragen dafür: Was ist der Input (Massenaufstellung + Plan)? Welches Tool müsste die Werte aus dem
Plan extrahieren (Wiederverwendung von M07)? Wie würde ein Soll/Ist-Abgleich als Ausgabe aussehen (z. B.
Ampel-Markierung bei Abweichung)?

Musterdaten für den Soll/Ist-Abgleich: [../musterdaten/massenaufstellung.csv](../musterdaten/massenaufstellung.csv)
gegen [../musterdaten/beispiel-plan.pdf](../musterdaten/beispiel-plan.pdf) — enthält bewusst 1 kleine
Abweichung (Büro 102), 1 größere Abweichung (Besprechungsraum) und 1 im Plan fehlenden Raum (Lager).

→ Übung siehe [uebung.md](uebung.md).

## Machbarkeit & nächste Ausbaustufen

Dies ist Tag 2 eines 2-Tage-Einstiegs — der realistische nächste Schritt ist ein Pilotprojekt mit
EFG-eigenen Testdaten, kein fertiges Produkt am Ende dieser Schulung.

## Trainer-Showcase

- **Ausgangslage (10 Min):** Unterschied zu Use Case 1 herausarbeiten.
- **Konzeptionelle Skizze (35 Min):** Kleingruppen bilden, Leitfragen an die Wand projizieren, während
  der Bearbeitung durch den Raum gehen.
- **Umfrage:** Machbarkeits-Einschätzung (1–5) je Teilaspekt (Extraktion, Abgleich, automatisierte
  Weiterverarbeitung).
- **Diskussion Machbarkeit & Ausbaustufen (15 Min):** Erwartungshaltung klarstellen.

## Leitfragen

Beantwortet die Fragen zuerst selbst, bevor ihr sie aufklappt.

<details>
<summary>Was ist der Kernunterschied zwischen Use Case 1 (Datenextraktion) und Use Case 2 (Aufmaßprüfung)?</summary>

UC1 = reine Extraktion. UC2 = Soll/Ist-Abgleich zweier Quellen (Massenaufstellung vs. Plan).

</details>

<details>
<summary>Welches Tool aus Use Case 1 lässt sich für Use Case 2 wiederverwenden?</summary>

Das Extraktions-Tool für Plan-Daten aus M07.

</details>

<details>
<summary>Nennt einen typischen Befund einer Aufmaßprüfung anhand der Musterdaten.</summary>

Kleine Abweichung, größere Abweichung oder ein im Plan fehlender Raum.

</details>
