# MEGN 301 — Mechanical Integration & Design: Master Reference Document

**Author:** Adam Duran, Assistant Teaching Professor  
**Institution:** Colorado School of Mines, Department of Mechanical Engineering  
**Course:** MEGN 301 — Mechanical Integration and Design  
**Semester:** Spring 2026

## Overview

A comprehensive 171-page reference document covering the complete design-build process for junior-level mechanical engineering students. The document integrates systems engineering theory with practical hardware design, organized around the V-Model lifecycle framework.

## Structure

| Part | Chapters | Content |
|------|----------|---------|
| **I: The Design-Build Process** | 1–6 | Problem definition, requirements, concept generation, V&V, integration, O&M |
| **II: Technical Reference** | 7–12 | Connectors, power supplies/motors/pumps, power architecture, fasteners/bearings, power transmission, injection molding DFM |
| **III: Major Project Milestones** | 13–15 | PDR, CDR, and FDR deliverables, evaluation criteria, and checklists |
| **Back Matter** | — | Glossary (50+ terms), References (25 sources) |

## Building the PDF

Requires a LaTeX distribution with `pdflatex` (e.g., TeX Live, MiKTeX).

```bash
# Three passes for cross-references and table of contents
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
```

### Required LaTeX Packages

The document uses standard packages available in most TeX distributions:

- `geometry`, `fancyhdr`, `titlesec`, `titletoc` — page layout and headers
- `tcolorbox` — colored tip/warning/concept boxes
- `tabularx`, `booktabs`, `longtable` — professional tables
- `amsmath`, `amssymb`, `siunitx` — equations and units
- `graphicx`, `xcolor[table]` — figures and colors
- `hyperref`, `cleveref` — cross-references and hyperlinks
- `enumitem`, `multicol` — list formatting
- `placeins`, `needspace` — float and page-break control

## File Structure

```
├── MEGN301_Compiled_Course_References_and_Notes.tex    # Main document
├── README.md
├── .gitignore
├── Concept Generation/                                  # Ch 3 figures (4 PNGs)
├── Designing for Injection Molding/                     # Ch 12 figures (4 PNGs)
├── Electrical and Fluid Connectors/                     # Ch 7 figures (7 PNGs)
├── Mechanical Fasteners and Bearings/                   # Ch 10 figures (3 PNGs)
├── Mechanical Power Transmission/                       # Ch 11 figures (4 PNGs)
├── Ops and Maintenance/                                 # Ch 6 figures (4 PNGs)
├── Power Architecture/                                  # Ch 9 figures (4 PNGs)
├── Power Supplies, Motors, and Pumps/                   # Ch 8 figures (4 PNGs)
├── Problem Statement and Stakeholder Engagement/        # Ch 1 figures (4 PNGs)
├── Project Milestones/                                  # Part III figures (1 PNG)
├── Requirements and Architecture/                       # Ch 2 figures (4 PNGs)
├── Subsystem Integration/                               # Ch 5 figures (4 PNGs)
└── Verification, Validation, and Test Plans/            # Ch 4 figures (4 PNGs)
```

**Total: 1 `.tex` file + 51 `.png` figures across 13 directories**

## Key Features

- **V-Model Framework** — Central organizing principle linking requirements to verification
- **GreenShield Case Study** — Running example (frost protection system) threaded through all chapters
- **Sprint-to-Chapter Mapping** — Direct alignment with MEGN 301 7-sprint project structure
- **Bottom Line Summaries** — Each chapter opens with a 2–3 sentence takeaway
- **Tiered Practice Questions** — Labeled C (Comprehension), A (Application), CT (Critical Thinking)
- **Industry Cross-References** — INCOSE SEH, NASA SP-2016-6105, IEEE, SAE, ASME standards
- **Artifact Progression Table** — Master matrix showing how 14 deliverables evolve from PDR → CDR → FDR
- **Comprehensive Glossary** — 50+ acronyms and key terms

## License

© 2026 Adam Duran, Colorado School of Mines. All rights reserved.
