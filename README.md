# thaumazo

This is a multi-purpose style file.

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
It also requires some `MnSymbol` fonts.

In particular, if using XeTeX, you will need to remove the part of the style file below or to add `MnSymbol7.otf` and `MnSymbol10.otf` to the font book on your computer.
```latex
\ifxetex
  \font\ten=MnSymbol10
  \font\seven=MnSymbol7
  \let\complement\relax
  \newcommand\complement{\text{\ten\char"2201}}
  \newcommand\complementss{\text{\seven\char"2201}}%for superscript
\fi
```

### General use

One might use thaumazo in the following way.
```latex
\documentclass[twoside]{article}

\def\ttitle{Motives}%optional
\def\tteacher{Pierre Deligne}%optional

\usepackage[course]{thaumazo}
...
```

[comment]: <> (### Behaviour of `\maketitle`)
[comment]: <> (### Options)
[comment]: <> (θαυμάζω)
