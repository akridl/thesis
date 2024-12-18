# Thesis

This repository contains LaTeX source code of [the thesis text](thesis.pdf).

## Template

The template used for the thesis is an official template provided by the Masaryk
University, from [Fithesis4](https://www.overleaf.com/latex/templates/fithesis4-for-the-faculty-of-informatics-at-the-masaryk-university-in-brno/qmrtczzjvpfv) family.

## Modularization

In order to split the source code into several files, **subfiles** package is
being used. For more info, see an [official Overleaf docs](https://www.overleaf.com/learn/latex/Multi-file_LaTeX_projects).

Once the subfiles package is added, actual paste of the content from another
file is done using _\subfile_ directive. For instance, to create new chapter,
it is enough to do simply:

```tex
\chapter{Introduction}
\subfile{chapters/introduction/main}
```

where **chapters/introduction/main** is the path to the file which should be
placed in the position where the corresponding _\subfile_ directive was used.

