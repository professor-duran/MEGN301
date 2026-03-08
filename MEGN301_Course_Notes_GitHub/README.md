# MEGN 301 — Mechanical Integration & Design: Course Materials

**Author:** Adam Duran, Assistant Teaching Professor  
**Institution:** Colorado School of Mines, Department of Mechanical Engineering  
**Course:** MEGN 301 — Mechanical Integration and Design  
**Semester:** Spring 2026

---

## 📥 Download the Latest PDFs

| Document | Link |
|----------|------|
| **Compiled Course Notes** (171 pages) | [⬇ Download](../../releases/tag/latest) |
| **Web Viewer** | [🌐 Open](https://YOUR_USERNAME.github.io/MEGN310/) |

> **Students:** Bookmark the links above — they always point to the latest version.

---

## Overview

A comprehensive reference document covering the complete design-build process for junior-level mechanical engineering students. Organized around the V-Model lifecycle framework with a running GreenShield case study.

## Document Structure

| Part | Chapters | Content |
|------|----------|---------|
| **I: The Design-Build Process** | 1–6 | Problem definition, requirements, concept generation, V&V, integration, O&M |
| **II: Technical Reference** | 7–12 | Connectors, power/motors/pumps, power architecture, fasteners/bearings, power transmission, injection molding |
| **III: Major Project Milestones** | 13–15 | PDR, CDR, FDR deliverables and evaluation criteria |
| **Back Matter** | — | Glossary (50+ terms), References (25 sources) |

## Automatic PDF Compilation

This repository uses **GitHub Actions** to automatically compile PDFs whenever you push changes to `.tex` or image files.

### How it works

```
Push .tex or .png changes
    ↓
GitHub Actions triggers automatically
    ↓
TeX Live compiles all .tex files → PDFs
    ↓
Three outputs:
  1. Build artifacts   (Actions tab, 90-day retention)
  2. GitHub Pages      (https://YOUR_USERNAME.github.io/MEGN310/)
  3. Latest Release    (github.com/YOUR_USERNAME/MEGN310/releases/tag/latest)
```

### Smart triggers

The pipeline **only runs** when content files change (`.tex`, `.png`, `.jpg`). Editing the README, LICENSE, or other non-content files does **not** trigger a rebuild.

### Adding a new document

To add a second document (e.g., a Student Project Guide):

1. Create `MEGN301_Student_Project_Guide.tex` in the repo root
2. Edit `.github/workflows/build-pdfs.yml` and uncomment the second `root_file` line
3. Push — the pipeline will compile both documents and publish both PDFs

### First-time setup

Before the pipeline works, enable these settings once:

1. **Workflow permissions:** Settings → Actions → General → Workflow permissions → **Read and write permissions** → Save
2. **GitHub Pages:** Settings → Pages → Source → **GitHub Actions**

## Building Locally

```bash
# Requires TeX Live or MiKTeX with pdflatex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
pdflatex MEGN301_Compiled_Course_References_and_Notes.tex
```

## File Structure

```
├── .github/workflows/build-pdfs.yml          # CI/CD pipeline
├── MEGN301_Compiled_Course_References_and_Notes.tex
├── README.md
├── .gitignore
├── Concept Generation/                        (4 PNGs)
├── Designing for Injection Molding/           (4 PNGs)
├── Electrical and Fluid Connectors/           (7 PNGs)
├── Mechanical Fasteners and Bearings/         (3 PNGs)
├── Mechanical Power Transmission/             (4 PNGs)
├── Ops and Maintenance/                       (4 PNGs)
├── Power Architecture/                        (4 PNGs)
├── Power Supplies, Motors, and Pumps/         (4 PNGs)
├── Problem Statement and Stakeholder Engagement/  (4 PNGs)
├── Project Milestones/                        (1 PNG)
├── Requirements and Architecture/             (4 PNGs)
├── Subsystem Integration/                     (4 PNGs)
└── Verification, Validation, and Test Plans/  (4 PNGs)
```

**Total: 1 `.tex` + 51 `.png` figures across 13 directories**

## Key Features

- **V-Model Framework** — Central organizing principle linking requirements to verification
- **GreenShield Case Study** — Running example threaded through all chapters
- **Sprint-to-Chapter Mapping** — Direct alignment with 7-sprint project structure
- **Colorblind-Safe Figures** — Wong (2011) palette with redundant line-style encoding
- **Bottom Line Summaries** — Each chapter opens with a concise takeaway
- **Tiered Practice Questions** — C (Comprehension), A (Application), CT (Critical Thinking)
- **Artifact Progression Table** — Master matrix showing 14 deliverables across PDR → CDR → FDR
- **Comprehensive Glossary** — 50+ acronyms and key terms

## License

© 2026 Adam Duran, Colorado School of Mines. All rights reserved.
