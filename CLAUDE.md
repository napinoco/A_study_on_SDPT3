# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a LaTeX academic project documenting the algorithm and implementation of SDPT3, a MATLAB solver for semidefinite-quadratic-linear programming.
The main document is a technical report written in English with mathematical content.

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

- `main_en.tex` - Main English LaTeX document (now modularized with \input commands)
- `section01_notations.tex` - Section 1: Mathematical notations and definitions
- `section02_problem_definition.tex` - Section 2: Primal and dual problem formulation
- `section03_interior_point_method.tex` - Section 3: Infeasible primal-dual path-following interior-point method
- `section04_predictor_corrector.tex` - Section 4: Predictor-corrector method
- `section05_sparsity_exploitation.tex` - Section 5: Sparsity exploitation techniques
- `section06_other_computation.tex` - Section 6: Other computational techniques
- `section07_summary.tex` - Section 7: Algorithm summary
- `appendix_a.tex` - Appendix A: Guide to equation derivations
- `references.bib` - Bibliography file with academic references
- `latexmkrc` - LaTeX build configuration (uses platex/pbibtex for Japanese compatibility)
- `backup/` - Contains backup versions of documents including Japanese version

## Key Document Components

The document is now modularized for easier editing and management:
- The original large `main_en.tex` file has been split into 8 separate section files
- Each section file contains complete LaTeX content for its respective section
- All mathematical notation, equations, labels, and cross-references are preserved
- The main file uses `\input{}` commands to include all section files

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