# Latex Template

This is a latex template for the dissertation that I did for my project in
M.Sc.

## Quickstart

### Requirements

- pdflatex
- biber
- texlive (full version is preferable)
- pygments

Look
[here](https://blog.wizardsoftheweb.pro/syntax-highlighting-in-latex-with-minted/)
to get code highlighting working in latex.

### Creating pdf

Use the `make` command to generate a pdf. If for some reason it doesn't work
and you have to look at the errors run this command separately:

```
pdflatex -shell-escape report.tex
```

General workflow is to do the following:

```
make
make clean
```

To force rebuild the pdf execute

```
make -B
```

### Changes you have to make

- The variables like author name are in `report.tex`. Edit those and you should
be good to go.
- Individual pages are in `pages` folder
- Chapters and Appendix are in `chapters` folder
- resources like images are in `res` folder
- bibliography is `report.bib`
