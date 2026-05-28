# Teacher-guided AI-assisted development of virtual physics laboratories: classroom case studies in secondary physics

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20425377.svg)](https://doi.org/10.5281/zenodo.20425377)

Public proof-of-concept and evidence repository for the paper:

> Teacher-guided AI-assisted development of virtual physics laboratories: classroom case studies in secondary physics

## Citation and DOI

This repository is archived on Zenodo and assigned a DOI for long-term preservation and citation.

**DOI:** https://doi.org/10.5281/zenodo.20425377

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
│   ├── figures/
│   │   ├── simulations/
│   │   │   ├── figure_diffraction_simulation_interface.png
│   │   │   ├── figure_transformer_simulation_interface.png
│   │   │   └── figure_lcr_simulation_interface.png
│   │   │
│   │   ├── manuscript/
│   │   │   └── figures used in the journal paper
│   │   │
│   │   └── classroom_examples/
│   │       └── classroom screenshots and poll summaries
│   │
│   ├── student_work/
│   │   ├── diffraction/
│   │   │   └── anonymized student response samples
│   │   │
│   │   ├── transformer/
│   │   │   └── anonymized student response samples
│   │   │
│   │   └── lcr/
│   │       └── anonymized student response samples
│   │
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
- Simulation screenshots intended for manuscript figures are stored in `assets/figures/simulations/`
- Example anonymized student submissions are stored in `assets/student_work/`
- Earlier simulation and worksheet versions are preserved to document the iterative teacher--AI co-development process described in the paper.

## Build

From the repository root:

```sh
cd docs/manuscript
latexmk -pdf main.tex
```

If `latexmk` is not available, compile manually using:

```sh
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## Notes

- The repository preserves earlier simulation and worksheet versions to document the iterative teacher--AI co-development process discussed in the manuscript.
- Student examples included in the repository are anonymized classroom samples intended solely for educational and research documentation.
- The repository functions both as a reproducibility archive for the paper and as a practical resource for physics teachers interested in AI-assisted virtual laboratory development.
