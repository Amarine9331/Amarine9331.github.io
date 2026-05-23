# Hantavirus Molecular Diagnostics Portfolio Notebook

This repository contains a Quarto/Markdown-style academic notebook:

- `hantavirus_taqman_assay_design.qmd` - source notebook
- `report.html` - rendered HTML output
- `hantavirus_taqman_assay_design.ipynb` - Jupyter/Colab-compatible notebook

The notebook is an educational portfolio case study about hantavirus phylogeny,
epidemiology, and hypothetical TaqMan-style assay design for molecular
diagnostics. It uses the 2026 MV Hondius Andes virus cluster as a motivating
public-health example, while avoiding operational primer/probe sequences,
bench protocols, or clinical testing instructions.

## Render

```bash
quarto render hantavirus_taqman_assay_design.qmd --to html
```

## Use With Colab or Jupyter

The notebook includes non-executing Python-style scaffolding for portfolio
presentation. Open `hantavirus_taqman_assay_design.ipynb` in Jupyter or upload
it to Colab.

To regenerate the notebook:

```bash
quarto render hantavirus_taqman_assay_design.qmd --to ipynb
```

or

```bash
jupytext --to ipynb hantavirus_taqman_assay_design.qmd
```
