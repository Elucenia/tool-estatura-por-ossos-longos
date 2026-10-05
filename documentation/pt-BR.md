<!-- ELUCENIA technical documentation · estatura-por-ossos-longos · pt-BR · no clinical/professional/rights approval -->

# Estatura por ossos longos (Trotter e Gleser)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/estatura-por-ossos-longos)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Sexo

`sexo`

- `F` — Feminino
- `M` — Masculino

### Osso medido

`osso`

- `fem` — Fêmur (comprimento máximo)
- `tib` — Tíbia
- `fib` — Fíbula
- `hum` — Úmero
- `rad` — Rádio
- `ulna` — Ulna

### Comprimento do osso

`comp`

cm · intervalo: 10–70

### Idade estimada (opcional, para correção)

`idade`

anos · opcional · intervalo: 18–100

## Edição do método

Trotter Gleser 1952 American Whites; correçãoidade 1951\>30 anos 0,06 cm/ano; populaçãooriginal restrita

## Fórmula documentada

Estatura (cm) = coeficiente × comprimento do osso (cm) + constante, pelas equações de Trotter e Gleser (1952) para o grupo "American Whites".

Correção pela idade: acima de 30 anos, subtrair 0,06 cm por ano (Trotter e Gleser, 1951).

## Limites e população

Estas regressões pertencem à população histórica e à definição de comprimento ósseo da edição selecionada; não são universais para todas as ancestralidades ou idades. Meça em cm e documente o osso e a técnica. Jantz 1995 identificou que a tíbia usada por Trotter excluía o maléolo; aplicar o comprimento padrão produziu superestimação média de 2,5–3 cm. Não misture definições de medida nem corrija o osso automaticamente. As tabelas originais de coeficientes e o ajuste etário não foram integralmente conferidos nesta revisão.

## Referências

- [Trotter M, Gleser GC. Estimation of stature from long bones of American Whites and Negroes. Am J Phys Anthropol, 1952.](https://doi.org/10.1002/ajpa.1330100407)

- [Trotter M, Gleser GC. The effect of ageing on stature. Am J Phys Anthropol, 1951.](https://doi.org/10.1002/ajpa.1330090307)

- [Jantz RL, Hunt DR, Meadows L. The measure and mismeasure of the tibia: implications for stature estimation. J Forensic Sci, 1995.](https://doi.org/10.1520/JFS15379J)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
