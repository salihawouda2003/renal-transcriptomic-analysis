[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/salihawouda2003/renal-transcriptomic-analysis/blob/main/renal_allograft_transcriptomics.ipynb)

# renal-transcriptomic-analysis
Computational analysis of renal allograft transcriptomics (GSE36059) to identify molecular biomarkers of transplant rejection. Built with Python and Google Colab.

# Renal Allograft Rejection: Transcriptomic Pipeline

### Project Context
This project was developed to bridge the gap between clinical wet-lab observations and scalable computational biology. Based on my experience in a renal transplant laboratory, I am building this pipeline to automate the identification of genetic signatures associated with acute rejection.

### Objective
To process high-dimensional transcriptomic data from the **GSE36059** dataset (400+ kidney biopsy samples) and identify significant biomarkers that distinguish stable grafts from T-cell mediated rejection.

**Key Results:** 
* Identified a high-confidence interferon-gamma signature (CXCL9, CXCL10, CXCL11) with a >2.0 Log2 Fold Change, consistent with established clinical biomarkers for T-cell mediated rejection.

### Technical Implementation
* **Platform:** Google Colab / Python 3.10
* **Data Retrieval:** `GEOparse` for direct NCBI Gene Expression Omnibus integration.
* **Analysis Stack:** `Pandas` for data wrangling, `Matplotlib/Seaborn` for visualization, and `Scipy` for statistical validation.

## Project Milestones

### Phase 1: Data Ingestion & Environment
- [x] Automated retrieval of 400+ clinical samples via NCBI GEO API.
- [x] Environment setup with bioinformatics-specific dependencies.

### Phase 2: Statistical Analysis & Clinical Annotation
- [x]  Developed a "Surgical" metadata parser to isolate diagnostic results from clinical notes.
- [x]  Calculated Log2 Fold Change (LFC) to measure rejection signal intensity.
- [x]  Mapped Affymetrix Probe IDs to human-readable **Gene Symbols**.
#### Discovery Visualization:
![Biomarker Distribution](https://colab.research.google.com/drive/1BkVbksWCeJInRwjkc_vwJfxyH6YRH8yJ#scrollTo=uO2hLHeCRlQT/content/biomarker_distribution.png)

### Phase 3: Advanced Visualization (In Progress)
- [x]  Current: Ranked Biomarker Bar Plots.
- Next: Generating high-resolution **Volcano Plots** and **Heatmaps** for pathway analysis.

## How to Run
1. Open `renal_allograft_transcriptomics.ipynb` in Google Colab.
2. Run all cells to fetch data directly from the NCBI server and generate current biomarker lists.
