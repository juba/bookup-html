# bookup-html custom quarto format

[![Publish examples](https://github.com/juba/bookup-html/actions/workflows/publish.yml/badge.svg)](https://github.com/juba/bookup-html/actions/workflows/publish.yml)


`bookup` is a custom [quarto](https://quarto.org) HTML format based on the Roboto font family. It provides both a light and dark theme, and should be suitable for single documents, book projects and website projects.

## Screenshots


<img src="screenshots/single_light.png" style="width: 250px; border: 1px solid #AAA;">
<img src="screenshots/single_dark.png" style="width: 250px; border: 1px solid #AAA;">


## Installation and usage

To use this custom format, first install the extension at the root directory of your project:

```bash
quarto add juba/bookup-html
```

And add the format to your YAML configuration, along with other HTML format options if needed:

```yaml
format:
    bookup-html:
        toc: true
        toc-depth: 3
```


Even simpler, you can also directly install the extensions and generate a sample qmd file from a template with:

```bash
quarto use template juba/bookup-html
```


## Format Options


Currently `bookup` provides the following options:

- `embed-fonts` : if set to `true`, fonts are included locally with the document. If set to `false`, they are downloaded from Google Web Fonts. Not that if you use `self-contained: true`, fonts are embedded inside the resulting HTML even if `embed-fonts` is `false`.


## Credits

This format is derived from the original [bookdown](https://bookdown.org) theme, adapted for the online french book [Introduction à R et au tidyverse](https://juba.github.io/tidyverse).

