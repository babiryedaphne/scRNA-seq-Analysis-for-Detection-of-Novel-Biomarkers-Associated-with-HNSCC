# scRNA-seq-Analysis-for-Detection-of-Novel-Biomarkers-Associated-with-HNSCC

## Table of Contents
- [Overview](#overview)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Data Input](#data-input)
- [Workflow](#workflow)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

---

## Overview

This repository contains an R Markdown script for analyzing single-cell RNA sequencing (scRNA-seq) data. The script performs various tasks such as preprocessing, clustering, differential expression analysis, and visualization. An HTML output of the executed script is also provided for easier interpretation and presentation.

---

## Requirements

* R version 4.0.0 or higher
* RStudio (highly recommended)
* Libraries:
  - reticulate
  - Seurat
  - Matrix
  - SingleCellExperiment
  - rstudioapi
  - stringr
  - BiocManager
  - R.utils
  - DropletUtils
  - scuttle
  - tidyverse
  - knitr
  - robustbase
  - scater
  - scran
  - corral
  - bluster
  - igraph
  - pathfindR.data
  - AUCell
  - pheatmap
  - gridExtra
  - org.Hs.eg.db
  - limma
  - BiocNeighbors
  - batchelor
  - celldex
  - SingleR
  - edgeR

---

## Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/YourUsername/scRNA-seq-analysis.git
    ```

2. Open R or RStudio and install the required packages:

    ```R
    # Install packages from CRAN
    install.packages(c("reticulate", "Matrix", "rstudioapi", "stringr", "R.utils", "tidyverse", "knitr", "robustbase", "pheatmap", "gridExtra"))

    # Install packages from Bioconductor
    if (!requireNamespace("BiocManager", quietly = TRUE))
        install.packages("BiocManager")

    BiocManager::install(c("Seurat", "SingleCellExperiment", "DropletUtils", "scuttle", "scater", "scran", "corral", "bluster", "igraph", "pathfindR.data", "AUCell", "org.Hs.eg.db", "limma", "BiocNeighbors", "batchelor", "celldex", "SingleR", "edgeR"))
    ```

---

## Usage

1. Open the `your_script_name.Rmd` file in RStudio.

2. **Important**: Change the file path in the `list.files("Data/GSE139324_RAW")` line to point to your specific data directory.

3. Run the R Markdown script. An HTML output file will also be generated upon execution.

---

## Data Input

The data should be located in a folder named `Data/GSE139324_RAW`. The script automatically reads the files from this directory.
The data used for this project is publicly available at the Gene Expression Omnibus (GEO) website, accession number GSE139324. 

---

## Workflow

The pipeline consists of the following steps:

1. Data Loading
2. Data Preprocessing
3. Quality Control
4. Normalisation
5. Feature Selection
6. Batch Correction & Dimensional Reduction
8. Clustering
9. Marker Gene Detection
10. Cell Type Annotation
11. Differential Expression Analysis between Conditions

---

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

## Acknowledgements

Thanks to the creators of the utilized R packages and all contributors to this project.

---

## Contact

If you have any questions, feel free to reach out:

- **GitHub**: [@babiryedaphne](https://github.com/babiryedaphne/scRNA-seq-Analysis-for-Detection-of-Novel-Biomarkers-Associated-with-HNSCC.git)

---

Feel free to add, remove, or modify sections as you see fit for your project. This should give users a good idea of what your project is about, how to set it up, and how to use it.
