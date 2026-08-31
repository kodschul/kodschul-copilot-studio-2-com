# M09 Theorie: Use Case 2 — Aufmaßprüfung

## Lernziel

Ein Agenten-Konzept für einen Soll/Ist-Abgleich skizzieren und die Machbarkeit realistisch einschätzen.

## Dauer

Tag 2 · 15:00–16:15 · 75 Minuten

## Ausgangslage (10 Min)

Massenaufstellung (Liste mit erwarteten Mengen) muss gegen Pläne (meist PDF, teils DXF) geprüft
werden. Unterschied zu Use Case 1: hier geht es um **Abgleich/Prüfung**, nicht nur Extraktion.

## Konzeptionelle Skizze eines Prüf-Agenten (35 Min)

In Kleingruppen: Agent-Konzept skizzieren (kein vollständiger Build, da Zeit begrenzt). Leitfragen: Was
ist der Input (Massenaufstellung + Plan)? Welches Tool müsste die Werte aus dem Plan extrahieren
(Wiederverwendung von M07)? Wie würde ein Soll/Ist-Abgleich als Ausgabe aussehen (z. B.
Ampel-Markierung bei Abweichung)?

Musterdaten: [../musterdaten/massenaufstellung.csv](../musterdaten/massenaufstellung.csv) gegen
[../musterdaten/beispiel-plan.pdf](../musterdaten/beispiel-plan.pdf) — enthält bewusst 1 kleine
Abweichung (Büro 102), 1 größere Abweichung (Besprechungsraum) und 1 im Plan fehlenden Raum (Lager).

→ Übung siehe [uebung.md](uebung.md).

## Diskussion Machbarkeit & nächste Ausbaustufen (15 Min)

Klarstellen: dies ist Tag 2 eines 2-Tage-Einstiegs — realistischer nächster Schritt ist ein
Pilotprojekt mit EFG-eigenen Testdaten, kein fertiges Produkt am Ende der Schulung.

## Leitfragen

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
