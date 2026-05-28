# Teacher-guided AI-assisted development of virtual physics laboratories

Public proof-of-concept and evidence repository for the paper:

> Teacher-guided AI-assisted development of virtual physics laboratories: classroom case studies from secondary physics

## Repository structure

The repository is organized to separate manuscript files, simulation source code, worksheets, and supporting classroom evidence.

```text
teacher-guided-ai-virtual-physics-labs/
│
├── docs/
│   ├── manuscript/
│   │   ├── main.tex                # Current IOP manuscript source
│   │   ├── main.pdf                # Compiled manuscript PDF
│   │   ├── iopjournal.cls          # IOP journal class file
│   │   └── orcid.pdf               # ORCID asset used in manuscript
│   │
│   └── templates/
│       ├── iopjournal-template.tex # Original journal template
│       ├── iopjournal-guidelines.pdf
│       └── supporting template assets
│
├── simulations/
│   ├── diffraction/
│   │   ├── diffraction_sim_final.html
│   │   └── earlier development versions
│   │
│   ├── transformer/
│   │   ├── transformer_sim_final.html
│   │   └── earlier development versions
│   │
│   └── lcr/
│       ├── lcr_sim_final.html
│       └── earlier development versions
│
├── worksheets/
│   ├── diffraction/
│   │   ├── diffraction_worksheet_final.tex
│   │   └── earlier worksheet versions
│   │
│   ├── transformer/
│   │   └── transformer_worksheet_final.tex
│   │
│   └── lcr/
│       ├── lcr_worksheet_final.tex
│       └── earlier worksheet versions
│
├── assets/
│   ├── transcripts/
│   │   └── AI interaction archives and development conversations
│   │
│   ├── surveys/
│   │   └── student feedback and survey summaries
│   │
│   └── classroom_notes/
│       └── supporting implementation notes
│
└── README.md
```

### Main resources

- Final classroom-ready simulations are located in `simulations/*/*_final.html`
- Final worksheets are located in `worksheets/*/*_final.tex`
- The current manuscript source is `docs/manuscript/main.tex`
- The compiled manuscript PDF is `docs/manuscript/main.pdf`
- Earlier simulation and worksheet versions are preserved to document the iterative teacher--AI co-development process described in the paper.

## Build

From the repository root:

```sh
cd manuscript
latexmk -pdf main.tex
```

If `latexmk` is not available, run `pdflatex main.tex` from `manuscript/`.
