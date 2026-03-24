# MEGN 301 — Mechanical Integration & Design

**Colorado School of Mines | Department of Mechanical Engineering**

[![Build LaTeX PDFs](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml/badge.svg)](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml)

---

## Course Overview

MEGN 301 is the cornerstone design course in the mechanical engineering curriculum at Colorado School of Mines. Students learn a structured product design methodology — from identifying customer needs and developing engineering specifications through concept generation, prototyping, and design verification. The course bridges analytical coursework with hands-on practice, preparing students to approach open-ended mechanical design problems with confidence, rigor, and creativity.

---

## Documents

All documents are open educational resources and are automatically rebuilt on every push to `main` via GitHub Actions.

| Document | Description | Download |
|----------|-------------|----------|
| **Master Reference Document** | 23-chapter comprehensive reference covering design methodology, analysis techniques, prototyping, and professional practice | [PDF](https://raw.githubusercontent.com/professor-duran/MEGN301/main/megn301_master_reference.pdf) |
| **Student Guide** | Course logistics, schedules, assignment details, rubrics, and operational reference | [PDF](https://raw.githubusercontent.com/professor-duran/MEGN301/main/MEGN301_Student_Guide.pdf) |

---

## Repository Structure

```
MEGN301/
├── .github/workflows/
│   └── build-pdfs.yml                  GitHub Actions CI workflow
│
├── mrd/                                Master Reference Document (modular LaTeX)
│   ├── main.tex                           Driver file
│   ├── preamble.tex                       Packages, colors, custom environments
│   ├── .latexmkrc                         latexmk config (handles makeindex)
│   ├── frontmatter/                       Title page, preface, reading guide, safety
│   ├── chapters/                          23 numbered chapters + 3 part intros
│   ├── appendices/                        Glossary, references, appendices
│   └── master_figs/                       All figures (68 PNGs)
│
├── student_guide/                      Student Guide (modular LaTeX)
│   ├── MEGN301_Student_Guide.tex          Driver file
│   └── sections/                          13 section files
│
├── megn301_master_reference.pdf        Pre-built MRD (committed by CI)
├── MEGN301_Student_Guide.pdf           Pre-built Student Guide (committed by CI)
└── README.md
```

---

## Building Locally

Requires a TeX Live or MiKTeX installation with `pdflatex` and `makeindex`.

```bash
# Master Reference Document (3-pass for index and cross-references)
cd mrd && pdflatex main && makeindex main.idx -s indexstyle.ist && pdflatex main && pdflatex main

# Student Guide (2-pass)
cd student_guide && pdflatex MEGN301_Student_Guide && pdflatex MEGN301_Student_Guide
```

---

## Built With

- **LaTeX** — Typesetting and document preparation
- **GitHub Actions** — Continuous integration; PDFs rebuild automatically on every push to `main`
- **Modular document architecture** — Each chapter and section is an independent `.tex` file for parallel authoring

---

## License and Use

These materials are open educational resources developed at Colorado School of Mines. Documents are living resources that evolve each semester as the course is refined.

---

## Author

**Adam Duran** | Assistant Teaching Professor, PE, PMP | Department of Mechanical Engineering | Colorado School of Mines
