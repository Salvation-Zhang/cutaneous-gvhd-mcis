# Cutaneous GVHD MCIS transcriptomic analysis

This repository contains analysis code and curated gene sets for the manuscript:

**Cross-dataset transcriptomic analysis identifies a conserved myeloid-cytotoxic inflammation program associated with keratinocyte stress in human cutaneous GVHD**

## Overview

This project reanalyzes public human cutaneous graft-versus-host disease (GVHD) transcriptomic datasets to identify reproducible immune-injury programs across single-cell RNA-seq and bulk RNA-seq cohorts.

The analysis focuses on coordinated inflammatory myeloid/APC activation, cytotoxic T/NK effector activity, and keratinocyte injury/stress programs. A myeloid-cytotoxic inflammation score (MCIS) was derived from S100 inflammatory monocyte, IFN/APC myeloid, HLA-II antigen-presentation, and cytotoxic T/NK signatures.

## Public datasets

- GSE236264: discovery human acute cutaneous GVHD single-cell RNA-seq dataset
- GSE190338: independent human acute cutaneous GVHD single-cell RNA-seq validation dataset
- GSE157538: human chronic cutaneous GVHD bulk RNA-seq dataset used for tissue-level support of signature detectability and co-variation

## Repository contents

- `dataset_accessions.csv`: GEO accession numbers and dataset roles.
- `gene_sets/mcis_component_gene_sets.csv`: curated gene sets used to calculate MCIS component scores.
- `gene_sets/keratinocyte_injury_stress_gene_sets.csv`: curated gene sets used to score keratinocyte IFN response, epithelial stress/injury, and antigen-presentation activity.
- `gene_sets/ligand_receptor_pairs.csv`: focused candidate ligand-receptor pairs evaluated in exploratory immune-injury analyses.
- `scripts/`: analysis scripts for single-cell processing, signature scoring, MCIS calculation, bulk RNA-seq scoring, ligand-receptor prioritization, and figure generation.

## Analysis summary

The workflow includes:

1. Processing and annotation of the GSE236264 discovery single-cell RNA-seq dataset.
2. Reclustering and scoring of myeloid/APC and cytotoxic T/NK compartments.
3. Projection of discovery-derived signatures into the independent GSE190338 single-cell validation dataset.
4. Tissue-level scoring of MCIS component signatures in the GSE157538 bulk RNA-seq dataset.
5. Exploratory ligand-receptor prioritization using selected inflammatory, chemokine, cytokine, and alarmin-receptor axes.
6. Association analysis between MCIS and keratinocyte injury/stress programs.

## Notes

All transcriptomic datasets used in this study are publicly available from the Gene Expression Omnibus. No new sequencing data were generated.

The bulk RNA-seq dataset GSE157538 represents chronic cutaneous GVHD and was used as tissue-level support for signature detectability and co-variation rather than as stage-matched validation of the acute single-cell findings.

## Citation

If you use this repository, please cite the associated manuscript:

Zhang Y, Peng J. Cross-dataset transcriptomic analysis identifies a conserved myeloid-cytotoxic inflammation program associated with keratinocyte stress in human cutaneous GVHD.
