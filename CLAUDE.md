# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal CV for Vitali Vinahradski, written in LaTeX using the `moderncv` document class (classic style, blue color scheme). The repo contains a single `.tex` file and a headshot photo.

## Build

Compile the CV to PDF with:
```
pdflatex cv_vitali_vinahradski_one_page.tex
```

### Environment Setup (Ubuntu/Debian)
```
sudo apt-get install texlive-latex-base texlive-latex-extra texlive-fonts-recommended texlive-fonts-extra
```
- `texlive-latex-extra` provides the `moderncv` class
- `texlive-fonts-recommended` provides `lmodern`
- `texlive-fonts-extra` provides `fontawesome5` (required by moderncv v2.4.1)

## Key Files

- `cv_vitali_vinahradski_one_page.tex` — the entire CV source (single-page layout, A4)
- `vitali_vinahradski.jpg` — headshot photo positioned via `\includegraphics` in a `picture` environment

## LaTeX Notes

- The CV uses `moderncv` with `\moderncvstyle{classic}` and `\moderncvcolor{blue}`
- Page geometry is set to `left=1.5cm, right=1.5cm, top=2cm, bottom=2cm`
- The photo is manually placed using a `picture` environment (the built-in `\photo` command is commented out)
- Negative `\vspace` is used throughout to keep the CV to one page — be careful when adding content
