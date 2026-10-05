<!-- ELUCENIA technical documentation · estatura-por-ossos-longos · it · no clinical/professional/rights approval -->

# Statura dalle ossa lunghe (Trotter e Gleser)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/estatura-por-ossos-longos)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Sesso

`sexo`

- `F` — Femminile
- `M` — Maschile

### Osso misurato

`osso`

- `fem` — Femore (lunghezza massima)
- `tib` — Tibia
- `fib` — Perone
- `hum` — Omero
- `rad` — Radio
- `ulna` — Ulna

### Lunghezza dell’osso

`comp`

cm · intervallo: 10–70

### Età stimata (facoltativa, per correzione)

`idade`

anni · facoltativo · intervallo: 18–100

## Edizione del metodo

Trotter–Gleser 1952 American Whites; correzione d’età 1951 \>30 anni 0,06 cm/anno; popolazione originale limitata

## Formula documentata

Statura (cm) = coefficiente × lunghezza ossea (cm) + costante, con Trotter–Gleser (1952) per il gruppo “American Whites”.

Correzione per età: oltre 30 anni sottrarre 0,06 cm per anno (Trotter–Gleser, 1951).

## Limiti e popolazione

Queste regressioni si riferiscono alla popolazione storica e alla definizione di lunghezza ossea dell’edizione selezionata; non sono universali per tutte le ascendenze o età. Misurare in cm e documentare osso e tecnica. Jantz 1995 ha rilevato che la misura tibiale di Trotter escludeva il malleolo; usare la lunghezza standard sovrastimava la statura in media di 2,5–3 cm. Non mescolare definizioni di misura né correggere automaticamente l’osso. Le tabelle originali dei coefficienti e l’aggiustamento per età non sono stati interamente verificati in questa revisione.

## Riferimenti

- [Trotter M, Gleser GC. Estimation of stature from long bones of American Whites and Negroes. Am J Phys Anthropol, 1952.](https://doi.org/10.1002/ajpa.1330100407)

- [Trotter M, Gleser GC. The effect of ageing on stature. Am J Phys Anthropol, 1951.](https://doi.org/10.1002/ajpa.1330090307)

- [Jantz RL, Hunt DR, Meadows L. The measure and mismeasure of the tibia: implications for stature estimation. J Forensic Sci, 1995.](https://doi.org/10.1520/JFS15379J)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
