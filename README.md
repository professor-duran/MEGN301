# MEGN 301 — Mechanical Integration & Design

**Author:** Adam Duran, Assistant Teaching Professor  
**Institution:** Colorado School of Mines, Department of Mechanical Engineering  
**Semester:** Spring 2026

## Overview

A comprehensive course materials package for MEGN 301, including a 173-page Master Reference Document covering the V-Model design-build lifecycle and electromechanical technical reference, plus a 25-page Student Companion Guide with sprint-by-sprint FAQ, tips, and common pitfall warnings.

## Repository Contents

| File / Directory | Description |
|-----------------|-------------|
| `MEGN301_Compiled_Course_References_and_Notes.tex` | Master Reference Document (Parts I–II, 12 chapters, 173 pages) |
| `MEGN301_Student_Guide.tex` | Student companion guide (25 pages, 33 FAQs, 22 Pro Tips, 16 Common Pitfalls) |
| `master_figs/` | Figures for the Master Reference Document (56 PNGs) |

## Building the PDFs

Both documents are compiled automatically via GitHub Actions on every push. Download the latest PDFs from the [Releases](../../releases) page, the [Actions](../../actions) tab, or the [course website](https://professor-duran.github.io/MEGN301/).

To build locally:

```bash
# Master Reference Document (three passes for cross-references)
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex

# Student Guide (two passes for table of contents)
pdflatex MEGN301_Student_Guide.tex
pdflatex MEGN301_Student_Guide.tex
```

## License

© 2026 Adam Duran, Colorado School of Mines. All rights reserved.
