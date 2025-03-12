# Validation of a Mitochondrial Polygenic Score for Parkinson’s Disease

`🦋 GP2 ❤️ Open Science 😍🦋`

[![DOI](https://zenodo.org/badge/947381299.svg)](https://doi.org/10.5281/zenodo.15013764)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Last Updated:** February 2025

## Summary

This is the online repository for the short report titled ***"Validation of a Mitochondrial Polygenic Score for Parkinson’s Disease"***. Mitochondrial polygenic scores (MGS), quantify the cumulative impact of multiple genetic variants associated with mitochondrial function. They may explain variability in disease status and clinical phenotypes in complex diseases like Parkinson’s disease. This study aims to evaluate the association of our MGS with PD status and AAO for both iPD and LRRK2-PD across a large, multi-ancestry cohort (i.e. GP2 dataset).

## Data Statement

- All GP2 data are hosted in collaboration with the Accelerating Medicines Partnership in Parkinson's Disease and are available via application on the website. The GP2 PD case and control data are available via the GP2 website ([https://gp2.org](https://gp2.org); release 6: [https://doi.org/10.5281/zenodo.10472143](https://doi.org/10.5281/zenodo.10472143)). Genotyping imputation, quality control, ancestry prediction, and processing were performed using GenoTools (v1.0.0), publicly available on GitHub

## Helpful Links 
* [GP2 Website](https://gp2.org/)
    * [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
* [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
    * [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)


## Repository Orientation
* Analyses discussed in the manuscript can be found in this repository:
    * The 1st notebook titled `00_gp2_mgs_iPD_ANCESTRY` contains codes that we used to calculate the MGS and analyse its association with disease status and age at onset for patients with idiopathic PD in the European cohort. This notebook can be recycled to analyse other ancestry groups simply by changing the group names whenever necessary.
    * The 2nd notebook titled `01_gp2_mgs_LRRK2` contains codes that we used to analyse the associations of our MGS with disease status and age at onset specifically for patients with LRRK2-PD. It assumes that you have already gone through the 1st notebook (for at least 1 ancestry) and have a list of LRRK2 variants that you are interested in testing.

```bash
THIS_REPO
├── LICENSE
├── README.md
└── analyses
    └── GP2
        ├── 00_gp2_mgs_iPD_ANCESTRY
        └── 01_gp2_mgs_LRRK2
```



## Analysis Notebooks
*  Languages: Python, bash, and R

|**Directory** |     **Notebooks**       |                                 **Description**                          |
|:------------:|:-----------------------:|:------------------------------------------------------------------------:|
| `GP2/`       |`00_gp2_mgs_iPD_ANCESTRY`     | Calculating MGS and analysing associations in iPD for European population|
| `GP2/`       |`01_gp2_mgs_LRRK2`       | Analysing associations in LRRK2-PD                                       |


## Software


|       **Software**                | **Version(s)** |           **Resource URL**                                           |   **RRID**     |                                                               **Notes**                                               |
|:---------------------------------:|:--------------:|:--------------------------------------------------------------------:|:--------------:|:---------------------------------------------------------------------------------------------------------------------:|
| Python Programming Language       |3.10            |http://www.python.org/                                                | RRID:SCR_008394| pandas; numpy; seaborn; matplotlib; statsmodel; used for general data wrangling/plotting/analyses                     |
|R Project for Statistical Computing|4.4.2           |http://www.r-project.org/                                             | RRID:SCR_001905| tidyverse; dplyr; tidyr; ggplot; car; data.table; pROC; wesanderson used for general data wrangling/plotting/analyses |
|PLINK                              |1.9 and 2.0     |http://www.nitrc.org/projects/plink                                   | RRID:SCR_001757| used for genetic analyses                                                                                             |
|GATK (Mutect2)                     | 4.3.0.0        |https://gatk.broadinstitute.org/hc/en-us/articles/360037593851-Mutect2| RRID:SCR_001876| call somatic SNVs and indels via local assembly of haplotypes                                                         |
---

