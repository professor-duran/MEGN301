# MEGN 301 — Mechanical Integration & Design

**Colorado School of Mines · Department of Mechanical Engineering**

[![Build LaTeX PDFs](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml/badge.svg)](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml)

## Latest Documents

| Document | Download |
|----------|----------|
| **Master Reference Document** | [📥 Download PDF](https://raw.githubusercontent.com/professor-duran/MEGN301/main/megn301_master_reference.pdf) |
| **Student Guide** | [📥 Download PDF](https://raw.githubusercontent.com/professor-duran/MEGN301/main/MEGN301_Student_Guide.pdf) |

> PDFs are automatically rebuilt on every push to `main` via GitHub Actions.

## Repository Structure
```
mrd/                                 Master Reference Document (modular LaTeX)
├── main.tex                            Driver file
├── preamble.tex                        Packages, colors, custom environments
├── .latexmkrc                          latexmk config (handles makeindex)
├── frontmatter/                        Title page, preface, reading guide, safety
├── chapters/                           23 numbered chapters + 3 part intros
├── appendices/                         Glossary, references, appendices
└── master_figs/                        All figures (68 PNGs)

student_guide/                       Student Guide (modular LaTeX)
├── MEGN301_Student_Guide.tex           Driver file
└── sections/                           13 section files
```

## Building Locally
```bash
# Master Reference Document (3-pass for index)
cd mrd && pdflatex main && makeindex main.idx -s indexstyle.ist && pdflatex main && pdflatex main

# Student Guide (2-pass)
cd student_guide && pdflatex MEGN301_Student_Guide && pdflatex MEGN301_Student_Guide
```

## Author

**Adam Duran** · Assistant Teaching Professor · PE, PMP · March 2026
