# quarto-eisvogel Format

This quarto extension is based on the wonderful [Eisvogel template](https://github.com/Wandmalfarbe/pandoc-latex-templ). 

## Installing

```bash
quarto use template lukfor/quarto-eisvogel
```

This will install the extension and create an example qmd file that you can use as a starting place for your article.

You could test the creates qmd file with

```bash
quarto preview my-file.qmd
```

## Using

```
---
title: Eisvogel Template
format:
  eisvogel-pdf:
    titlepage: false
    toc: false
    number-sections: false
author: John Doe
date: last-modified
bibliography: references.bib
---
```


## Format Options

A list of all variables can be found [here](https://github.com/Wandmalfarbe/pandoc-latex-template?tab=readme-ov-file#custom-template-variables).

We changed the following default values:

```
toc: true
number-sections: true
block-heading: false
toc-own-page: true
link-citations: true
titlepage: true
csl: "ieee-with-url.csl"
colorlinks: true
classoption: oneside
```

## Example

Here is the source code for a minimal sample document: [template.qmd](template.qmd).

