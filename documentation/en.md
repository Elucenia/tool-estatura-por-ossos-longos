<!-- ELUCENIA technical documentation · estatura-por-ossos-longos · en · no clinical/professional/rights approval -->

# Stature from long bones (Trotter and Gleser)

[conditions, sources and permissions](https://elucenia.org/en/tools/estatura-por-ossos-longos)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Sex

`sexo`

- `F` — Female
- `M` — Male

### Measured bone

`osso`

- `fem` — Femur (maximum length)
- `tib` — Tibia
- `fib` — Fibula
- `hum` — Humerus
- `rad` — Radius
- `ulna` — Ulna

### Bone length

`comp`

cm · range: 10–70

### Estimated age (optional, for correction)

`idade`

years · optional · range: 18–100

## Method edition

Trotter–Gleser 1952 American Whites; age correction 1951 \>30 years 0.06 cm/year; restricted original population

## Documented formula

Stature (cm) = coefficient × bone length (cm) + constant, using Trotter–Gleser (1952) equations for the “American Whites” group.

Age correction: above 30 years, subtract 0.06 cm per year (Trotter–Gleser, 1951).

## Limits and population

These regressions belong to the historical population and bone-length definition of the selected edition; they are not universal across ancestries or ages. Measure in cm and document the bone and technique. Jantz 1995 found that Trotter’s tibial measurement excluded the malleolus; using the standard length overestimated stature by 2.5–3 cm on average. Do not mix measurement definitions or automatically correct the bone. The original coefficient tables and age adjustment have not been fully checked in this review.

## References

- [Trotter M, Gleser GC. Estimation of stature from long bones of American Whites and Negroes. Am J Phys Anthropol, 1952.](https://doi.org/10.1002/ajpa.1330100407)

- [Trotter M, Gleser GC. The effect of ageing on stature. Am J Phys Anthropol, 1951.](https://doi.org/10.1002/ajpa.1330090307)

- [Jantz RL, Hunt DR, Meadows L. The measure and mismeasure of the tibia: implications for stature estimation. J Forensic Sci, 1995.](https://doi.org/10.1520/JFS15379J)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
