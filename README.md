# MEGN 301 — Mechanical Integration & Design

**Colorado School of Mines · Department of Mechanical Engineering**

[![Build LaTeX PDFs](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml/badge.svg)](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml)

## Latest Documents

| Document | Download |
|----------|----------|
| **Master Reference Document** | [megn301_master_reference.pdf](megn301_master_reference.pdf) |
| **Student Guide** | [MEGN301_Student_Guide.pdf](MEGN301_Student_Guide.pdf) |

> PDFs are automatically rebuilt on every push to `main` via GitHub Actions.

## Repository Structure

```
megn301_mrd/                         Master Reference Document (modular LaTeX)
├── main.tex                            Driver file
├── megn301.sty                         Shared style package
├── indexstyle.ist                      Index formatting
├── frontmatter/                        Title page, preface, reading guide, safety
├── chapters/                           23 numbered chapters + 3 part intros
├── backmatter/                         Glossary, references, appendices
└── master_figs/                        All figures (68 PNGs)

megn301_sg/                          Student Guide (modular LaTeX)
├── main.tex                            Driver file
├── megn301.sty                         Shared style package
└── sections/                           13 section files
```

## Building Locally

```bash
# Master Reference Document (3-pass for index)
cd megn301_mrd
pdflatex main && makeindex main.idx -s indexstyle.ist && pdflatex main && pdflatex main

# Student Guide (2-pass)
cd megn301_sg
pdflatex main && pdflatex main
```

## Author

**Adam Duran** · Assistant Teaching Professor · PE, PMP · March 2026
