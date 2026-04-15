# MEGN 301 — Mechanical Integration & Design

**Colorado School of Mines | Department of Mechanical Engineering**

[![Build LaTeX PDFs](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml/badge.svg)](https://github.com/professor-duran/MEGN301/actions/workflows/build-pdfs.yml)
![Built](https://img.shields.io/badge/built-2026--03--24-blue)
![Version](https://img.shields.io/badge/version-v1.0.0-green)

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

## Document Structure (23 Chapters)

### Part I: The Design-Build Process
1. **Problem Definition & Stakeholder Engagement** — Identifying the right problem, stakeholder analysis, concept of operations, competitive benchmarking
2. **Value Proposition & Triple Bottom Line** — Feasibility, desirability, viability, sustainability (FDVS) framework; competitive analysis; cost analysis
3. **Writing Requirements & Defining Architecture** — SDRD, functional decomposition, trade studies, FMEA, interface definitions
4. **Concept Generation & Early Design** — Morphological charts, decision matrices, prototype types, BOM development
5. **Verification, Validation & Test Plans** — V&V concepts, TAID methods, test procedures, VCRM, boundary testing
6. **Subsystem Integration** — Integration sequence planning, N² diagrams, debugging, configuration management
7. **Operations & Maintenance** — Lifecycle cost, serviceability, quick-start guides, maintenance manuals
8. **Post-Build Testing, Verification & Validation** — Test execution workflow, non-conformance reports, root cause analysis
9. **End of Life & System Retirement** — Design for recycling, design for disassembly, disposal planning

### Part II: Technical Reference
10. **Electrical & Fluid Connectors** — Connector family selection, failure modes, NPT vs BSP standards
11. **Power Supplies, Motors & Pumps** — Motor/pump sizing, driver selection, battery sizing, belt conveyor examples
12. **Power Architecture & Circuit Safety** — Power budget design, grounding strategy, protection circuits, EMI management
13. **Electronics Fundamentals, Safety & Component Selection** — Ohm's Law, KVL/KCL, voltage dividers, electrical safety
14. **Principles of Sensors and Actuators** — Transduction principles, six-criteria selection framework, signal conditioning
15. **Mechanical Fasteners & Bearings** — Metric fastener specification, threaded inserts, bearing selection, torque guidelines
16. **Mechanical Power Transmission** — Motor-to-load matching, gear design (including 3D-printed gears), speed/torque trade-offs
17. **Designing for Injection Molding** — Six DFM rules, uniform walls, draft angles, radii, tooling economics
18. **Printed Circuit Board Design Fundamentals** — PCB structure, grounding and decoupling, trace width, bring-up protocol
19. **Microcontrollers & the ESP32** — MCU fundamentals, GPIO pin map, communication protocols, firmware best practices
20. **Systematic Debugging and Troubleshooting** — Debugging pyramid, five-step protocol, bottom-up integration verification

### Part III: Major Project Milestones
21. **Preliminary Design Review (PDR)** — "Should this design work?" Problem verification, requirements validation, concept selection rationale
22. **Critical Design Review (CDR)** — "Will this design work?" Detailed design completeness, manufacturability, verification procedures
23. **Final Design Review (FDR)** — "How well did it work?" System validation, as-built documentation, lessons learned, operations package

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

## Adoption and License

These materials are open educational resources developed at Colorado School of Mines and licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You are free to **share** and **adapt** the materials for any purpose, including commercially, provided you give appropriate credit. See [LICENSE](LICENSE) for full details.

**Suggested attribution:**
> MEGN 301: Mechanical Integration & Design course materials by Adam W. Duran, Colorado School of Mines, used under CC BY 4.0. Source: https://github.com/professor-duran/MEGN301

Documents are living resources that evolve each semester as the course is refined. If you adopt these materials, I'd love to hear about it -- please reach out so I can learn from your experience.

---

## Author and Contact

**Adam W. Duran** | Assistant Teaching Professor, PE, PMP | Department of Mechanical Engineering | Colorado School of Mines

Email: [aduran@mines.edu](mailto:aduran@mines.edu)
Website: [adamwduran.com](https://adamwduran.com)
