[![DOI](https://zenodo.org/badge/1437449504.svg)](https://doi.org/10.5281/zenodo.23742256)

# Linear Algebra: Study Guide

**N. I. Tolipov.** *Linear Algebra: Study Guide.* Fergana, 2026.
UDC 512.64(075.8), LBC 22.143ya73.

An open-access study guide covering the 24 topics of the course "Linear Algebra": matrices and determinants, systems of linear equations, vectors and analytic geometry, linear and Euclidean spaces, linear operators, quadratic forms and iterative methods for linear systems.

Each topic contains the necessary theory, examples solved in full detail, applications in information security and short computations in Python, Maple and Mathcad. More than two thousand exercises for independent work are included, all with answers. The guide is intended for university students of information security, computer engineering and other engineering programmes.

## Download

- [Read or download the PDF](Linear_Algebra_Study_Guide_English.pdf)
- Archived version with DOI: https://doi.org/10.5281/zenodo.23742256

## How to cite

N. I. Tolipov. Linear Algebra: Study Guide. Fergana, 2026. https://doi.org/10.5281/zenodo.23742256

## License

This work is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0): https://creativecommons.org/licenses/by/4.0/

## Contents

- 24 topics, each with definitions, theorems, worked examples, applications in information security, short Python/Maple/Mathcad computations and exercises for independent work.
- Answers to all exercises: the section "Answers to the Exercises" at the end of the book (`qismlar/javoblar.tex`).

## Building from source

The book is written in LaTeX (XeLaTeX, A5).

**Locally:** `latexmk main.tex`, or run `xelatex main.tex` twice (for the table of contents).

**On Overleaf:**

1. Download this repository as a ZIP (Code → Download ZIP).
2. Overleaf → New Project → Upload Project → upload the ZIP.
3. Menu → Compiler: XeLaTeX, Main document: `main.tex`.
4. Recompile. There is no need to comment out any chapter with `%`.

The book is set up to fit into the 10-second limit of the free Overleaf plan: `xelatex` runs only once each time (no `.aux` file is used; the table of contents is taken from `qismlar/mundarija.mnd` and `output.mnd`).

Settings made for speed (do not change them):

- the math font is `newtxmath` (instead of `unicode-math`);
- frames use the `framed` package (instead of `mdframed`);
- `hyperref` is switched off (it is not needed for a printed book);
- figures are ready-made PDFs (their sources are in `rasmlar/manba/`);
- the font's TeX ligatures are switched off: type the characters ’, –, “ ” directly in the text.

To view a single chapter: open `boblar/bob3.tex` and click Recompile from that file.

### Repository structure

```
main.tex                    the whole book
latexmkrc                   XeLaTeX settings for latexmk/Overleaf
qismlar/mundarija.mnd       ready-made table of contents (for the first compilation)
sozlamalar/                 preamble, environments, hyphenation, book data
qismlar/                    title page, introduction, conclusion, references, javoblar.tex
boblar/bob1..bob5.tex       chapters; boblar/bobN/mXX.tex: the 24 topics
rasmlar/                    figures
```
