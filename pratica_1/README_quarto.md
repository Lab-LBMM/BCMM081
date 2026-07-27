# Template quarto (gerado com Claude - modelo Opus 5)

```bash
quarto preview intro_R.qmd   # recarrega a cada save
quarto render  intro_R.qmd   # gera o HTML final
```

Pacotes R usados: `knitr`, `ggplot2`, `countdown`

```r
install.packages(c("knitr", "ggplot2", "countdown"))
```

## O que editar primeiro

- **Cores e fontes:** as cinco variáveis no topo de cada `.scss`. Mudar ali muda o deck inteiro.
- **Cabeçalho YAML:** título, autor, `footer`, `logo`.
- **`lang: pt-BR`** controla os rótulos automáticos (callouts, "Figura", etc.).

## Recursos de revealjs usados nos templates

| Recurso | Como se escreve |
|---|---|
| Revelar linha por linha | `#\| code-line-numbers: "\|1\|2-3"` |
| Anotar linhas de código | `# <1>` no código + lista numerada abaixo |
| Saída ao lado do código | `#\| output-location: column-fragment` |
| Saída só no clique | `#\| output-location: fragment` |
| Gráfico em slide próprio | `#\| output-location: slide` |
| Mostrar o erro em vez de falhar | `#\| error: true` |
| Pausa dentro do slide | `. . .` numa linha sozinha |
| Lista item a item | `::: {.incremental}` |
| Duas colunas | `::: {.columns}` + `::: {.column width="50%"}` |
| Notas do apresentador | `::: {.notes}` (tecla `S`) |
| Texto gigante que se ajusta | `::: {.r-fit-text}` |
| Slide de seção colorido | `## Título {.divider}` ou `{background-color="#3D6B4A"}` |
| Fonte menor no slide | `## Título {.smaller}` |
| Slide rolável | `## Título {.scrollable}` |

## Teclas durante a apresentação

`S` notas · `F` tela cheia · `O` visão geral · `B` lousa · `C` desenhar sobre o slide · `E` modo impressão (depois Ctrl+P → PDF)