# renal-transcriptomic-analysis
Computational analysis of renal allograft transcriptomics (GSE36059) to identify molecular biomarkers of transplant rejection. Built with Python and Google Colab.

# Renal Allograft Rejection: Transcriptomic Pipeline

### Project Context
This project was developed to bridge the gap between clinical wet-lab observations and scalable computational biology. Based on my experience in a renal transplant laboratory, I am building this pipeline to automate the identification of genetic signatures associated with acute rejection.

### Objective
To process high-dimensional transcriptomic data from the **GSE36059** dataset (400+ kidney biopsy samples) and identify significant biomarkers that distinguish stable grafts from T-cell mediated rejection.

### Technical Implementation
* **Platform:** Google Colab / Python 3.10
* **Data Retrieval:** `GEOparse` for direct NCBI Gene Expression Omnibus integration.
* **Analysis Stack:** `Pandas` for data wrangling, `Matplotlib/Seaborn` for visualization, and `Scipy` for statistical validation.

### Current Milestone: Phase 1
- [x] Repository initialized and linked to Google Colab.
- [x] Automated retrieval of 400+ clinical samples.
- [ ] Data Normalization & Log2 Transformation (In Progress).
- [ ] Differential Expression Analysis & Volcano Plotting.
