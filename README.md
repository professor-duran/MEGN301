# MEGN 301 — Mechanical Integration & Design

**Colorado School of Mines · Department of Mechanical Engineering**

[![Build LaTeX PDFs](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml/badge.svg)](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml)

Course notes and reference materials for MEGN 301: Mechanical Integration & Design.

## 📄 Latest Documents

| Document | Download |
|----------|----------|
| **Master Reference Document** | [📥 megn301_master_reference.pdf](megn301_master_reference.pdf) |
| **Student Guide** | [📥 MEGN301_Student_Guide.pdf](MEGN301_Student_Guide.pdf) |

> PDFs are automatically rebuilt on every push to `main` via GitHub Actions.

## Repository Contents

```
├── megn301_master_reference.tex      LaTeX source — Master Reference Document
├── MEGN301_Student_Guide.tex         LaTeX source — Student Guide
├── *_notes.tex                       Individual module lecture notes (12 modules)
├── master_figs/                      Figures for the master reference document
└── fig_*/                            Figures for individual module presentations
```

## Document Structure

### Part I: The Design-Build Process
1. Problem Definition & Stakeholder Engagement
2. Value Proposition & Triple Bottom Line
3. Writing Requirements & Defining Architecture
4. Concept Generation & Early Design
5. Verification, Validation & Test Plans
6. Subsystem Integration
7. Operations & Maintenance
8. Post-Build Testing, Verification & Validation
9. End of Life & System Retirement

### Part II: Technical Reference
10. Electrical & Fluid Connectors
11. Power Supplies, Motors & Pumps
12. Power Architecture & Circuit Safety
13. Mechanical Fasteners & Bearings
14. Mechanical Power Transmission
15. Designing for Injection Molding
16. Printed Circuit Board Design Fundamentals
17. Microcontrollers & the ESP32

### Part III: Major Project Milestones
18. Preliminary Design Review (PDR)
19. Critical Design Review (CDR)
20. Final Design Review (FDR)

## Building Locally

Requires `pdflatex` with `tcolorbox`, `tikz`, `enumitem`, `booktabs`, `tabularx`, `fancyhdr`, and `hyperref` packages.

```bash
pdflatex megn301_master_reference.tex
pdflatex megn301_master_reference.tex   # run twice for TOC
```

## Author

**Adam Duran** · Assistant Teaching Professor · PE, PMP  
Department of Mechanical Engineering · Colorado School of Mines
