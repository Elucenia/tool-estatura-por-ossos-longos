<!-- ELUCENIA technical documentation · estatura-por-ossos-longos · de · no clinical/professional/rights approval -->

# Körpergröße aus langen Knochen (Trotter und Gleser)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/estatura-por-ossos-longos)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Geschlecht

`sexo`

- `F` — Weiblich
- `M` — Männlich

### Gemessener Knochen

`osso`

- `fem` — Femur (maximale Länge)
- `tib` — Tibia
- `fib` — Fibula
- `hum` — Humerus
- `rad` — Radius
- `ulna` — Ulna

### Knochenlänge

`comp`

cm · Bereich: 10–70

### Geschätztes Alter (optional, zur Korrektur)

`idade`

Jahre · optional · Bereich: 18–100

## Fassung der Methode

Trotter–Gleser 1952 American Whites; Alterskorrektur 1951 \>30 Jahre 0,06 cm/Jahr; eingeschränkte Ursprungspopulation

## Dokumentierte Formel

Körpergröße (cm) = Koeffizient × Knochenlänge (cm) + Konstante, nach Trotter–Gleser (1952) für die Gruppe „American Whites“.

Alterskorrektur: über 30 Jahre pro Jahr 0,06 cm abziehen (Trotter–Gleser, 1951).

## Grenzen und Population

Diese Regressionen beziehen sich auf die historische Population und die Definition der Knochenlänge in der gewählten Ausgabe; sie sind nicht für alle Abstammungsgruppen oder Altersgruppen universell gültig. Messen Sie in cm und dokumentieren Sie Knochen und Technik. Jantz 1995 stellte fest, dass Trotters Tibiamessung den Malleolus ausschloss; die Standardlänge führte im Mittel zu einer Überschätzung der Körperhöhe um 2,5–3 cm. Vermischen Sie keine Messdefinitionen und korrigieren Sie den Knochen nicht automatisch. Die Originalkoeffiziententabellen und die Alterskorrektur wurden in dieser Prüfung nicht vollständig abgeglichen.

## Referenzen

- [Trotter M, Gleser GC. Estimation of stature from long bones of American Whites and Negroes. Am J Phys Anthropol, 1952.](https://doi.org/10.1002/ajpa.1330100407)

- [Trotter M, Gleser GC. The effect of ageing on stature. Am J Phys Anthropol, 1951.](https://doi.org/10.1002/ajpa.1330090307)

- [Jantz RL, Hunt DR, Meadows L. The measure and mismeasure of the tibia: implications for stature estimation. J Forensic Sci, 1995.](https://doi.org/10.1520/JFS15379J)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Geschätzte Körpergröße von 168,5 ± 3,27 cm (1 Standardfehler)

| Ergebnisdetails | |
| --- | --- |
| Gleichung (Femur) | 2,38 × 45,0 + 61,41 = 168,5 cm |
| Bereich ± 2 Standardfehler (~95%) | 162,0 bis 175,0 cm |


### 2

Geschätzte Körpergröße von 163,0 ± 3,66 cm (1 Standardfehler)

| Ergebnisdetails | |
| --- | --- |
| Gleichung (Tibia) | 2,90 × 35,0 + 61,53 = 163,0 cm |
| Bereich ± 2 Standardfehler (~95%) | 155,7 bis 170,4 cm |


### 3

Geschätzte Körpergröße von 170,3 ± 4,05 cm (1 Standardfehler)

| Ergebnisdetails | |
| --- | --- |
| Gleichung (Humerus) | 3,08 × 33,0 + 70,45 = 172,1 cm |
| Alterskorrektur (0,06 cm/Jahr über 30) | −1,8 cm |
| Bereich ± 2 Standardfehler (~95%) | 162,2 bis 178,4 cm |


### 4

Geschätzte Körpergröße von 159,2 ± 4,24 cm (1 Standardfehler)

| Ergebnisdetails | |
| --- | --- |
| Gleichung (Radius) | 4,74 × 22,0 + 54,93 = 159,2 cm |
| Bereich ± 2 Standardfehler (~95%) | 150,7 bis 167,7 cm |

