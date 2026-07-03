# Scripts

This folder contains analysis scripts for the cutaneous GVHD MCIS transcriptomic analysis.

Suggested script organization:

- `01_scRNA_processing_GSE236264.R`: process and annotate the discovery single-cell RNA-seq dataset.
- `02_validation_GSE190338.R`: project discovery-derived signatures into the independent validation single-cell dataset.
- `03_bulk_scoring_GSE157538.R`: calculate tissue-level signature scores in bulk RNA-seq data.
- `04_mcis_scoring.R`: calculate MCIS component scores and integrated MCIS.
- `05_ligand_receptor_prioritization.R`: prioritize candidate ligand-receptor interactions.
- `06_figures.R`: generate figures and summary plots.

Scripts should be run after downloading the corresponding public GEO datasets. Large raw data files are not included in this repository.
