# Teacher-guided AI-assisted development of virtual physics laboratories

Working repository for the paper:

> Teacher-guided AI-assisted development of virtual physics laboratories: classroom case studies from secondary physics

## Repository structure

- `manuscript/` - current IOP manuscript source, class file, ORCID asset, and compiled PDF.
- `source_materials/` - classroom evidence and development materials used while preparing the paper.
- `source_materials/ai_transcripts/` - AI interaction archives and related media.
- `source_materials/surveys/` - student feedback and survey files.
- `source_materials/classroom_notes/` - supporting classroom notes.
- `journal_template/` - original IOP LaTeX template and author guidance.

## Build

From the repository root:

```sh
cd manuscript
latexmk -pdf main.tex
```

If `latexmk` is not available, run `pdflatex main.tex` from `manuscript/`.
