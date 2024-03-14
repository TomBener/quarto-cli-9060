[How to Pass Custom Metadata Value to LaTeX Partials?](https://github.com/quarto-dev/quarto-cli/discussions/9060)

```shell
quarto render test.qmd --to pdf
```

The cause is that the table environment `\begin{table}` should not be used in the LaTeX permeable. See the [answer](https://github.com/quarto-dev/quarto-cli/discussions/9060#discussioncomment-8775556) of @cderv. Also see the [documentation](https://quarto.org/docs/journals/templates.html#latex-partials) of Quarto and its [source code](https://github.com/quarto-dev/quarto-cli/tree/main/src/resources/formats/pdf/pandoc).
