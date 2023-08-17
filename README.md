# quarto-rug-slc

Materials for the Hello Quarto: A World of Possibilities (for Reproducible Publishing) talk at Harvard's CCB Seminar Series (2023-03-27)

## Abstract

Quarto is an open-source scientific and technical publishing system that unifies and extends the R Markdown ecosystem. This talk will introduce you to creating creating reproducible, computational documents, from course notes to journal publications to books and web pages with Quarto. Familiarity with R and RStudio will be helpful for following along with the demos, however, those who work with any computational documents in any language (e.g., Jupyter Notebooks with Python) will also find the content relevant, particularly since Quarto is language-agnostic and can be used to create dynamic content with any computing language.

## Setup notes

R 4.2.2 (2022-10-31) -- "Innocent and Trusting"
RStudio 2023.03.0+386 "Cherry Blossom"
Quarto 1.3.287
Packages: tidyverse, palmerpenguins, gt

## Demo

### Documents

- Open the simple Quarto document called `index.qmd` and edit it using the RStudio Visual Editor.
- Bold palmerpenguins and add link to https://allisonhorst.github.io/palmerpenguins/.
- Add code chunk options:
  - `fig-alt`
  - `echo: false` in `execute` in the YAML
  - `code-fold`
  - teaching tip: `echo: fenced`
- Add a figure and a table and cross reference them
- Add a citation: 10.1371/journal.pone.0090081

### Slides

- Change `format: revealjs`
- Add section headings: First level headings Introduction and Analysis, under Analysis a second level heading called Modeling
- Add columns to slides
- Reveal code with `echo: true`
  - teaching-tip: `code-line-numbers`
- Change `output-location` of figure

### Websites

- Add another document `about.qmd`
- Add `quarto.yml` 

```
project:
  type: website

website:
  title: "Hello Quarto"
  navbar:
    left:
      - index.qmd
      - talk.qmd
```

- Render
- Add other formats to index.qmd:

```
format:
  html: default
  pdf: default
```

- `publish quarto`

### Journal articles (time permitting)

- Go to https://quarto.org/docs/journals/templates.html

- Click on Quarto journals repo

- Create one with JASA template

my-awesome-paper

- Add a citation

First from Zotero
Welcome to the tidyverse
