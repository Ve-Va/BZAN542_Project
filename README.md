# BZAN542 Data Mining Project

This repository contains our analysis of the **Online Retail II** dataset from the UCI Machine Learning Repository.  The project explores customer purchasing behavior through clustering and association rule mining in R.

## Repository layout

```
├── data/              Raw dataset files (CSV and Excel)
├── trials/            R Markdown notebooks with the analysis
├── BZAN542_Final_Report_Group1.pdf  Final written report
├── ProjectPresentation_Group1.pptx  Presentation slides
├── ProposalPresentation_DataMining.pptx  Initial proposal slides
└── notes              Short notes about the dataset
```

- **data/** – Contains `online_retail_II.xlsx` and two CSV splits (`online_retail.csv` and `online_retail2.csv`).  They are provided for convenience; the Excel file is the full dataset.
- **trials/** – Houses all R Markdown (`.Rmd`) notebooks used during exploration.  Notebooks such as `CodeUpdate_Dec3_v2.Rmd` perform feature engineering (e.g., RFM metrics), clustering (k‑means, hierarchical, DBSCAN) and visualization.  Other notebooks (`CodeUpdate_AR_Clusters.Rmd`, `CodeUpdate_AR_Retail.Rmd`) apply association-rule mining with the `arules` package.
- **Report and slides** – Summarize the methodology and findings.  These are useful for a quick overview of the project results.

## Getting started

1. Install R (version 4.0 or later recommended) and the following packages:
   ```r
   install.packages(c("tidyverse", "arules", "arulesViz", "cluster", "scatterplot3d", "dbscan", "lubridate"))
   ```
2. Open any of the `.Rmd` files in `trials/` with RStudio (or run `rmarkdown::render()` from the command line) to reproduce the analyses.
3. The data files in `data/` are ~40–45 MB each, so ensure there is sufficient disk space before running the notebooks.

## Notes

The `notes` file briefly explains that `online_retail_II.xlsx` is the original dataset, while the two CSVs are splits for ease of loading in R.

Feel free to experiment with the notebooks or extend them with additional feature engineering and modeling techniques.
