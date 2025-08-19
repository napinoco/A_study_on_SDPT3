# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a LaTeX academic project documenting the algorithm and implementation of SDPT3, a MATLAB solver for semidefinite-quadratic-linear programming. The main document is a technical report written in English with mathematical content.

## Build Commands

The project uses Japanese LaTeX tools configured via `latexmkrc`:

```bash
# Compile the English version
latexmk -pdf main_en.tex

# Clean auxiliary files
latexmk -c main_en.tex

# Clean all generated files including PDF
latexmk -C main_en.tex
```

## Project Structure

- `main_en.tex` - Main English LaTeX document about SDPT3 algorithm
- `references.bib` - Bibliography file with academic references
- `latexmkrc` - LaTeX build configuration (uses platex/pbibtex for Japanese compatibility)
- `backup/` - Contains backup versions of documents including Japanese version

## Key Document Components

The main document includes:
- Mathematical notation and definitions for semidefinite programming
- Detailed algorithm descriptions with mathematical proofs
- Implementation details aligned with MATLAB SDPT3 solver
- Uses standard LaTeX packages: `amsmath`, `amssymb`, `algorithm`, `algorithmic`

## Important Notes

- The document uses complex mathematical notation including matrix operations, cones, and optimization theory
- Bibliography references key SDPT3 papers (Toh et al. 1999, 2003, 2012)
- Uses `scrartcl` document class for better typography

## Writing Guidelines

- Use academically correct and appropriate terminology in the field of mathematical optimization
- Avoid overly literary or excessively strong expressions
- Maintain formal academic writing style consistent with mathematical optimization literature
- Do not perform actions not explicitly requested
- Always confirm with the user when something seems necessary or when there are concerns

## Git Guidelines

- Keep commit messages simple and concise (single line)
- Avoid multi-line commit messages or detailed descriptions