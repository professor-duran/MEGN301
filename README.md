# MEGN 301 — Mechanical Integration & Design

**Author:** Adam Duran, Assistant Teaching Professor  
**Institution:** Colorado School of Mines, Department of Mechanical Engineering  
**Semester:** Spring 2026

---

## 📥 Download the Latest PDFs

| Document | Link |
|----------|------|
| **Compiled Course Notes** | [⬇ Latest Release](https://github.com/professor-duran/MEGN301/releases/tag/latest) |
| **Student Project Guide** | [⬇ Latest Release](https://github.com/professor-duran/MEGN301/releases/tag/latest) |
| **Web Viewer** | [🌐 professor-duran.github.io/MEGN301](https://professor-duran.github.io/MEGN301/) |

> **Students:** Bookmark the links above — they always point to the latest version.

---

## Document Structure

### Compiled Course Notes (171 pages)

| Part | Chapters | Content |
|------|----------|---------|
| **I: The Design-Build Process** | 1–6 | Problem definition, requirements, concept generation, V&V, integration, O&M |
| **II: Technical Reference** | 7–12 | Connectors, power/motors/pumps, power architecture, fasteners/bearings, power transmission, injection molding |
| **III: Major Project Milestones** | 13–15 | PDR, CDR, FDR deliverables and evaluation criteria |
| **Back Matter** | — | Glossary (50+ terms), References (25 sources) |

### Student Project Guide

Sprint-by-sprint companion guide with project-specific tips, calendar warnings, and deliverable checklists.

---

## Automatic PDF Compilation

PDFs are auto-compiled by GitHub Actions whenever `.tex` or image files change.

```
Push .tex or .png changes → GitHub Actions → TeX Live compiles → PDFs published to:
  1. GitHub Pages  (https://professor-duran.github.io/MEGN301/)
  2. Latest Release (github.com/professor-duran/MEGN301/releases/tag/latest)
  3. Build artifacts (Actions tab)
```

### First-time setup

1. **Settings → Actions → General → Workflow permissions** → **Read and write permissions** → Save
2. **Settings → Pages → Source** → **GitHub Actions** → Save

---

## Building Locally

```bash
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex

pdflatex MEGN301_Student_Guide.tex
pdflatex MEGN301_Student_Guide.tex
pdflatex MEGN301_Student_Guide.tex
```

---

## Repository Structure

```
├── .github/workflows/build-pdfs.yml               # CI/CD pipeline
├── MEGN301_Compiled_Course_References_and_Notes.tex  # Main course notes
├── MEGN301_Student_Guide.tex                       # Student project guide
├── README.md
├── .gitignore
├── presentations/                                  # 12 .pptx + 12 .docx transcripts
├── Concept Generation/                             # Figure directories (51 PNGs total)
├── Designing for Injection Molding/
├── Electrical and Fluid Connectors/
├── Mechanical Fasteners and Bearings/
├── Mechanical Power Transmission/
├── Ops and Maintenance/
├── Power Architecture/
├── Power Supplies, Motors, and Pumps/
├── Problem Statement and Stakeholder Engagement/
├── Project Milestones/
├── Requirements and Architecture/
├── Subsystem Integration/
└── Verification, Validation, and Test Plans/
```

## License

© 2026 Adam Duran, Colorado School of Mines. All rights reserved.
