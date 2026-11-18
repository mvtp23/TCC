# Concessão e Expansão do Aeroporto Internacional de Florianópolis

**Avaliação dos impactos sobre a atividade econômica entre 2013 e 2023**

Trabalho de Conclusão de Curso — Curso de Graduação em Ciências Econômicas, Universidade Federal
de Santa Catarina (2026).
Autor: Marcos Vinicius Thibes Petussi. Orientador: Prof. Guilherme Valle Moura, Dr.

Material da análise empírica do trabalho, estimada por Synthetic Difference-in-Differences (SDID).

- **Relatório (HTML):** [https://mvtp23.github.io/TCC/banca/](https://mvtp23.github.io/TCC/banca/),
  com texto, tabelas e gráficos. O código de cada bloco pode ser exibido pelo botão *Code*.
- **Código-fonte (R Markdown):** [`modelo_sdid.Rmd`](modelo_sdid.Rmd). Gera o relatório acima. Os
  dados brutos são baixados automaticamente das releases deste repositório.

## Como reproduzir

1. Instale o R e os pacotes:

   ```r
   install.packages(c("dplyr", "readxl", "nanoparquet", "ggplot2", "ggrepel", "rmarkdown"))
   install.packages("remotes"); remotes::install_github("synth-inference/synthdid")
   ```

2. Gere o relatório:

   ```r
   rmarkdown::render("modelo_sdid.Rmd")
   ```

Os dados são guardados em `data/` e os resultados em `outputs/`. A estimação completa leva
algumas horas.
