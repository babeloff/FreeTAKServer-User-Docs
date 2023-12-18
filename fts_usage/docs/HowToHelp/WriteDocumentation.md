# Write Documentation

This project houses the FreeTakServer (FTS) documentation.
It is written in Markdown and mkdirs.

## Dependencies

Here are the packages it uses:
These packages are available for `conda`.

```shell
mamba env create -y -f fts_usage/docs/HowToHelp/fts-doc-env.yml
```
This environment includes the packages needed to construct the document products.
```yaml
{!HowToHelp/fts-doc-env.yml!}
```

## Preview Document

Start a service to view the resulting document.
```shell
mkdocs serve
```

## Usage Notes

The markdown files are coordinated and supplemented by `mkdocs` and its plugins.
Some of the more important features of those plugins are presented here.

`mkdocs` is configured via the `mkdocs.yml` file.

### Awesome Pages

Each document directory should contain a `.pages`.
These `.pages` distribute the `nav:` element across the document rather than collecting them in the `mkdocs.yml` file.
This implies that `mkdocs.yml` should not contain a `nav:` element.

### Markdown Includes

This file contains a typical example.
The `fts-doc-env.yml` file mentioned above is itself included using this facility.

i.e.  
\```yml  
{\!HowToHelp/fts-doc-env.yml\!}  
\```

### Mike (multi-version support)

The `fts_user/docs/versions.json` is used to define the versions.

TODO: Explain how this is to be used.