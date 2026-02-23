# Análise de Queimadas no Brasil — Maio 2025

> Análise exploratória de focos de queimadas e incêndios no Brasil, desenvolvida na disciplina **Organização e Apresentação de Dados (GES109)** do curso de Estatística da Universidade Federal de Lavras (UFLA).

## Acesse os resultados

| Entrega | Link |
|---|---|
| Dashboard interativo | Link ainda não disponível |
| Relatório completo | *([link RPubs aqui](https://rpubs.com/luizalucio/explorando-focos-de-queimadas-e-incendios-no-br))* |

## Sobre os dados

Os dados foram obtidos no portal de dados abertos do **Programa Queimadas do INPE (Instituto Nacional de Pesquisas Espaciais)**, coletados em 26/05/2025.

- Fonte: [TerraBrasilis — Focos de Queimadas e Incêndios](https://terrabrasilis.dpi.inpe.br/queimadas/portal/dados-abertos/)
- Base original: América Latina — 131.180 observações, 16 variáveis
- Recorte utilizado: Brasil — 930 observações, 5 variáveis (data, estado, dias sem chuva, risco de fogo, bioma)

## O que foi analisado

- Ranking de estados por mediana de dias sem chuva
- Frequência de focos de queimadas por bioma
- Relação entre dias sem chuva e risco de fogo
- Mapa coroplético de risco médio por estado

## Tecnologias utilizadas

![R](https://img.shields.io/badge/R-276DC3?style=flat&logo=r&logoColor=white)
![Quarto](https://img.shields.io/badge/Quarto-75AADB?style=flat&logo=quarto&logoColor=white)

**Pacotes R:** `tidyverse` · `ggplot2` · `plotly` · `geobr` · `lubridate` · `knitr` · `abjutils` · `stringr`

## Como reproduzir localmente

1. Clone o repositório:
```bash
git clone https://github.com/luizalucio/analise-queimadas.git
cd analise-queimadas
```

2. Instale os pacotes necessários no R:
```r
install.packages(c("tidyverse", "ggplot2", "plotly", "geobr",
                   "lubridate", "knitr", "abjutils", "stringr"))
```

3. Renderize os arquivos (com internet, para o `geobr` baixar o shapefile na primeira vez):
```bash
quarto render meu-dashboard.qmd
quarto render relatorio-queimadas.qmd
```

> O arquivo `focos_mensal_202505.csv` precisa estar na mesma pasta que os `.qmd`.

## Autora

**Luíza Helena Pereira Lúcio**  
Estudante de Estatística — UFLA  
📧 luiza.lucio1@estudante.ufla.br  
🔗 [LinkedIn](https://www.linkedin.com/in/luizahplucio/) · [GitHub](https://github.com/luizalucio) · [Portfólio](https://luizalucio.github.io/meu-site)
