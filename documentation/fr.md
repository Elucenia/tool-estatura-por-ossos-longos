<!-- ELUCENIA technical documentation · estatura-por-ossos-longos · fr · no clinical/professional/rights approval -->

# Estimation de la stature par les os longs (Trotter et Gleser)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/estatura-por-ossos-longos)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Sexe

`sexo`

- `F` — Féminin
- `M` — Masculin

### Os mesuré

`osso`

- `fem` — Fémur (longueur maximale)
- `tib` — Tibia
- `fib` — Fibula
- `hum` — Humérus
- `rad` — Radius
- `ulna` — Ulna

### Longueur osseuse

`comp`

cm · intervalle: 10–70

### Âge estimé (facultatif, pour correction)

`idade`

ans · facultatif · intervalle: 18–100

## Édition de la méthode

Trotter–Gleser 1952 American Whites ; correction d’âge 1951 \>30 ans 0,06 cm/an ; population originale restreinte

## Formule documentée

Stature (cm) = coefficient × longueur osseuse (cm) + constante, selon Trotter–Gleser (1952) pour le groupe « American Whites ».

Correction d’âge : au-delà de 30 ans, soustraire 0,06 cm par an (Trotter–Gleser, 1951).

## Limites et population

Ces régressions correspondent à la population historique et à la définition de la longueur osseuse de l’édition sélectionnée ; elles ne sont pas universelles pour toutes les ascendances ou tous les âges. Mesurez en cm et documentez l’os et la technique. Jantz 1995 a constaté que la mesure tibiale de Trotter excluait la malléole ; l’emploi de la longueur standard surestimait la taille de 2,5–3 cm en moyenne. Ne mélangez pas les définitions de mesure et ne corrigez pas automatiquement l’os. Les tableaux originaux de coefficients et l’ajustement lié à l’âge n’ont pas été intégralement vérifiés dans cette revue.

## Références

- [Trotter M, Gleser GC. Estimation of stature from long bones of American Whites and Negroes. Am J Phys Anthropol, 1952.](https://doi.org/10.1002/ajpa.1330100407)

- [Trotter M, Gleser GC. The effect of ageing on stature. Am J Phys Anthropol, 1951.](https://doi.org/10.1002/ajpa.1330090307)

- [Jantz RL, Hunt DR, Meadows L. The measure and mismeasure of the tibia: implications for stature estimation. J Forensic Sci, 1995.](https://doi.org/10.1520/JFS15379J)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Taille estimée de 168,5 ± 3,27 cm (1 erreur standard)

| Détails du résultat | |
| --- | --- |
| Équation (fémur) | 2,38 × 45,0 + 61,41 = 168,5 cm |
| Intervalle ± 2 erreurs standard (~95%) | 162,0 à 175,0 cm |


### 2

Taille estimée de 163,0 ± 3,66 cm (1 erreur standard)

| Détails du résultat | |
| --- | --- |
| Équation (tibia) | 2,90 × 35,0 + 61,53 = 163,0 cm |
| Intervalle ± 2 erreurs standard (~95%) | 155,7 à 170,4 cm |


### 3

Taille estimée de 170,3 ± 4,05 cm (1 erreur standard)

| Détails du résultat | |
| --- | --- |
| Équation (humérus) | 3,08 × 33,0 + 70,45 = 172,1 cm |
| Correction selon l’âge (0,06 cm/an au-dessus de 30) | −1,8 cm |
| Intervalle ± 2 erreurs standard (~95%) | 162,2 à 178,4 cm |


### 4

Taille estimée de 159,2 ± 4,24 cm (1 erreur standard)

| Détails du résultat | |
| --- | --- |
| Équation (radius) | 4,74 × 22,0 + 54,93 = 159,2 cm |
| Intervalle ± 2 erreurs standard (~95%) | 150,7 à 167,7 cm |

