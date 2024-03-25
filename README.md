# quarto-eisvogel Format

This quarto extension is based on the wonderful [Eisvogel template](https://github.com/Wandmalfarbe/pandoc-latex-template). 

## Installing

```bash
quarto use template lukfor/quarto-eisvogel
```

This will install the extension and create an example qmd file that you can use as a starting place for your article.

You could test the creates qmd file with

```bash
quarto preview my-file.qmd
```

Et voilà, enjoy the clean result.

![Preview](screenshots/preview.png)

## Using

After you have installed the extension, you will have a new format called `eisvogel-pdf` available. You can use it and adapt it to your needs:

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

# Hello

wow, doesn't Eisvogel look beautiful?

```

You can also utilize `eisvogel-pdf` for writing books. Refer to the Quarto documentation and modify the format in the `_quarto.yml` file as follows:

```
project:
  type: book

book:
    title: "The Life and Achievements of John Doe"
    author: "Mario Rossi and Max Mustermann"
    date: "24. July 2023"
    chapters:
      - index.qmd
      - chapter1.qmd
      - chapter2.qmd
      - chapter3.qmd
      - chapter4.qmd
      - references.qmd 
bibliography: references.bib  

format:
  eisvogel-pdf:
    book: true
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

## Credits

Thanks to [@Wandmalfarbe](https://github.com/Wandmalfarbe/) for the beautiful [Eisvogel template](https://github.com/Wandmalfarbe/pandoc-latex-template).  🙏
