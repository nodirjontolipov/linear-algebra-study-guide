[![DOI](https://zenodo.org/badge/1437449504.svg)](https://doi.org/10.5281/zenodo.23742256)
# Linear Algebra — study guide (XeLaTeX, A5, final version)

## Opening on Overleaf
1. Overleaf → New Project → Upload Project → upload this zip file.
2. Menu → **Compiler: XeLaTeX**, **Main document: main.tex**.
3. Recompile. There is no need to comment out any chapter with `%`.

The book is set up to fit into the **10-second** limit of the free Overleaf
plan: xelatex runs only **once** each time (no .aux file is used; the table
of contents is taken from `qismlar/mundarija.mnd` and `output.mnd`).

Settings made for speed (do not change them):
- the math font is `newtxmath` (instead of unicode-math);
- frames use the `framed` package (instead of mdframed);
- `hyperref` is switched off (it is not needed for a printed book);
- figures are ready-made PDFs (their sources are in `rasmlar/manba/`);
- the font's TeX ligatures are switched off: type the characters **’**,
  **–**, **“ ”** directly in the text.

To view a single chapter: open `boblar/bob3.tex` and click Recompile from that file.

## Structure
```
main.tex                    the whole book
latexmkrc                   XeLaTeX settings for latexmk/Overleaf
qismlar/mundarija.mnd       ready-made table of contents (for the first compilation)
sozlamalar/                 preamble, environments, hyphenation, book data
qismlar/                    title page, introduction, conclusion, references, javoblar.tex
boblar/bob1..bob5.tex       chapters; boblar/bobN/mXX.tex — the 24 topics
rasmlar/                    figures
```

## Contents
- 24 topics, each with definitions, theorems, worked examples,
  applications in information security, short Python/Maple/Mathcad
  computations and exercises for independent work.
- Answers to all exercises: the section "Answers to the Exercises" at the
  end of the book (`qismlar/javoblar.tex`).

## Local compilation
`latexmk main.tex` or `xelatex main.tex` (twice, for the table of contents).
