<!-- ELUCENIA technical documentation · estatura-por-ossos-longos · es · no clinical/professional/rights approval -->

# Estatura a partir de huesos largos (Trotter y Gleser)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/estatura-por-ossos-longos)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Sexo

`sexo`

- `F` — Femenino
- `M` — Masculino

### Hueso medido

`osso`

- `fem` — Fémur (longitud máxima)
- `tib` — Tibia
- `fib` — Peroné
- `hum` — Húmero
- `rad` — Radio
- `ulna` — Cúbito

### Longitud del hueso

`comp`

cm · intervalo: 10–70

### Edad estimada (opcional, para corrección)

`idade`

años · opcional · intervalo: 18–100

## Edición del método

Trotter–Gleser 1952 American Whites; corrección por edad 1951 \>30 años 0,06 cm/año; población original restringida

## Fórmula documentada

Estatura (cm) = coeficiente × longitud ósea (cm) + constante, por Trotter–Gleser (1952) para el grupo “American Whites”.

Corrección por edad: por encima de 30 años, restar 0,06 cm por año (Trotter–Gleser, 1951).

## Límites y población

Estas regresiones corresponden a la población histórica y a la definición de longitud ósea de la edición seleccionada; no son universales para todas las ascendencias o edades. Mida en cm y documente el hueso y la técnica. Jantz 1995 identificó que la tibia usada por Trotter excluía el maléolo; usar la longitud estándar produjo una sobreestimación media de 2,5–3 cm de la estatura. No mezcle definiciones de medición ni corrija el hueso automáticamente. Las tablas originales de coeficientes y el ajuste por edad no se han comprobado íntegramente en esta revisión.

## Referencias

- [Trotter M, Gleser GC. Estimation of stature from long bones of American Whites and Negroes. Am J Phys Anthropol, 1952.](https://doi.org/10.1002/ajpa.1330100407)

- [Trotter M, Gleser GC. The effect of ageing on stature. Am J Phys Anthropol, 1951.](https://doi.org/10.1002/ajpa.1330090307)

- [Jantz RL, Hunt DR, Meadows L. The measure and mismeasure of the tibia: implications for stature estimation. J Forensic Sci, 1995.](https://doi.org/10.1520/JFS15379J)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Estatura estimada de 168,5 ± 3,27 cm (1 error estándar)

| Detalles del resultado | |
| --- | --- |
| Ecuación (fémur) | 2,38 × 45,0 + 61,41 = 168,5 cm |
| Intervalo ± 2 errores estándar (~95%) | 162,0 a 175,0 cm |


### 2

Estatura estimada de 163,0 ± 3,66 cm (1 error estándar)

| Detalles del resultado | |
| --- | --- |
| Ecuación (tibia) | 2,90 × 35,0 + 61,53 = 163,0 cm |
| Intervalo ± 2 errores estándar (~95%) | 155,7 a 170,4 cm |


### 3

Estatura estimada de 170,3 ± 4,05 cm (1 error estándar)

| Detalles del resultado | |
| --- | --- |
| Ecuación (húmero) | 3,08 × 33,0 + 70,45 = 172,1 cm |
| Corrección por edad (0,06 cm/año por encima de 30) | −1,8 cm |
| Intervalo ± 2 errores estándar (~95%) | 162,2 a 178,4 cm |


### 4

Estatura estimada de 159,2 ± 4,24 cm (1 error estándar)

| Detalles del resultado | |
| --- | --- |
| Ecuación (radio) | 4,74 × 22,0 + 54,93 = 159,2 cm |
| Intervalo ± 2 errores estándar (~95%) | 150,7 a 167,7 cm |

