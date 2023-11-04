# thaumazo

This is a multi-purpose LaTeX style file that I use to create documents.

One uses thaumazo by invoking `\usepackage{thaumazo}` in the preamble of a LaTeX document.
Generally speaking, one should not `\usepackage` too many packages beyond thaumazo; it is meant to encompass most of the commonly used LaTeX packages, and clashes are likely to occur otherwise.
Consulting the list of packages that this style file uses below may help you determine what you can add.
Also, the file is easy enough to read that manipulating it to one's needs shouldn't be too much of a problem.

### Required packages

Below is a list of packages that the style file calls.
```
tipa
xcolor
amsthm
amssymb
amsfonts
amsmath
microtype
graphicx
tikz
tikz-cd
wasysym
stackengine
fontenc
inputenc
beramono
regexpatch
fancyhdr
mathrsfs
hyperref
cleveref
geometry
imakeidx
```
It also requires some MnSymbol fonts.

### General use

One might use thaumazo in the following way.
```latex
\documentclass [twoside] {article}

\def \ttitle {Motives} % optional
\def \tteacher {Pierre Deligne} % optional

\usepackage [course] {thaumazo}

\begin {document}
...
```

### Behaviour of `\maketitle`


### Options


θαυμάζω was Greek for ``I am amazed.''
