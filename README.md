# MEGN 301: Mechanical Integration & Design — Course Materials

[![Build MEGN 301 PDFs](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml/badge.svg)](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml)

**Author:** Adam Duran, PE, PMP
**Institution:** Colorado School of Mines, Department of Mechanical Engineering
**Term:** Spring 2026

---

## Download PDFs

| Document | Description | Link |
|---|---|---|
| **Master Reference Document** | 270+ page comprehensive reference covering the design-build lifecycle, electromechanical subsystem design, and project milestones | [**Download PDF**](https://raw.githubusercontent.com/professor-duran/MEGN301/main/megn301_master_reference.pdf) |
| **Student Guide** | 30-page companion with FAQ, tips, common pitfalls, and sprint-by-sprint checklists | [**Download PDF**](https://raw.githubusercontent.com/professor-duran/MEGN301/main/MEGN301_Student_Guide.pdf) |

PDFs are auto-compiled by GitHub Actions on every push and committed to this branch.

---

## Repository Structure

```
MEGN301/
├── mrd/                             Master Reference Document (modular)
│   ├── main.tex                     Build entry point
│   ├── preamble.tex                 Packages, colors, custom environments
│   ├── .latexmkrc                   latexmk config (handles makeindex)
│   ├── frontmatter/
│   │   ├── titlepage.tex
│   │   ├── howto.tex
│   │   ├── reading_guide.tex
│   │   └── safety.tex
│   ├── chapters/
│   │   ├── ch01_problem_definition.tex
│   │   ├── ch02_value_proposition.tex
│   │   ├── ...
│   │   └── ch23_fdr.tex
│   ├── appendices/
│   │   ├── glossary.tex
│   │   ├── exam_reference.tex
│   │   ├── fifteen_mistakes.tex
│   │   ├── quick_reference_tables.tex
│   │   ├── references.tex
│   │   └── ...
│   └── master_figs/                 All PNG figures
├── student_guide/
│   ├── MEGN301_Student_Guide.tex    Build entry point
│   └── sections/
│       ├── philosophy.tex
│       ├── sprint1.tex ... sprint7.tex
│       ├── presentation.tex
│       ├── final_report.tex
│       ├── tips.tex
│       ├── sprint_checklist.tex
│       └── formulas.tex
├── .github/workflows/               GitHub Actions auto-build
├── megn301_master_reference.pdf      ← auto-built by CI
└── MEGN301_Student_Guide.pdf         ← auto-built by CI
```

## Editing Workflow

Each chapter is a self-contained `.tex` file. Edit any file under `mrd/` or `student_guide/`, commit, push. GitHub Actions recompiles **both** PDFs automatically.

**Fast local build of a single chapter:**
```bash
# Uncomment this line in mrd/main.tex:
#   \includeonly{chapters/ch15_fasteners}
cd mrd && latexmk -pdf main.tex    # ~5 seconds instead of ~60
```

Re-comment `\includeonly` before pushing.

## Building Locally

**Prerequisites:** TeX Live (full) or MacTeX, with `latexmk`

```bash
# Build MRD
cd mrd && latexmk -pdf main.tex

# Build Student Guide
cd student_guide && latexmk -pdf MEGN301_Student_Guide.tex
```
