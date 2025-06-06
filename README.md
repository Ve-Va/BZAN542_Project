# BZAN542 Data Mining Project

This repository contains our coursework for the **Online Retail II** data from the UCI Machine Learning Repository. It explores customer purchasing behavior using clustering and association rule mining in R.

## Repository structure

- **data/** – Raw dataset files (`online_retail_II.xlsx` and CSV splits). Each file is roughly 40–45 MB.
- **trials/** – R Markdown notebooks performing the analysis. Key notebooks include:
  - `CodeUpdate_Dec3_v2.Rmd` for data cleaning, feature engineering with RFM metrics, and clustering (k‑means, hierarchical, DBSCAN).
  - `CodeUpdate_AR_Clusters.Rmd` and `CodeUpdate_AR_Retail.Rmd` for association‑rule mining with the `arules` package.
  - `.zip` archives of older notebook versions for reference.
- **BZAN542_Final_Report_Group1.pdf** – Final written report.
- **ProjectPresentation_Group1.pptx** – Slides summarizing the results.
- **ProposalPresentation_DataMining.pptx** – Original project proposal.
- **notes** – Short notes describing the dataset splits.

## Running the analysis

1. Install R (version 4.0 or later) and required packages:
   ```r
   install.packages(c("tidyverse", "arules", "arulesViz",
                      "cluster", "scatterplot3d", "dbscan", "lubridate"))
   ```
2. Open any `.Rmd` file in `trials/` with RStudio or render it via `rmarkdown::render()` to reproduce the analysis.

## Learning more

- Review the notebooks to see how missing values and return transactions are handled.
- Examine the construction of RFM features and clustering steps for customer segmentation.
- Check the association‑rule notebooks for itemset analysis examples.
- Read the final report and presentation slides for a concise overview of the findings.

Feel free to extend the notebooks or automate parts of the analysis as you experiment.
