# pancreatic_cancer_ml_pipeline

This study is an exploration of various machine learning models (and the statistical comparison of these models) as they apply to patient health data with varying degrees and types of bias. The three datasets utilized in this analysis were obtained from the Prostrate, Lung, Colorectal, and Ovarian (PLCO) Cancer Trial; in this study, we work with pancreatic cancer data obtained as a corollary from the trial. The datasets each included health records for both cases (patients who had pancreatic cancer) and controls (patients who did not have pancreatic cancer).

The primary research objectives of this study are to develop a comprehensive machine learning pipeline encompassing a broad spectrum of models to be compared across datasets, as well as to assess various contributors of bias between datasets and how they can be handled in machine learning population-based cohort studies. 

This repository contains the Jupyter notebooks, and supplemental materials for our research paper on assessing machine learning bias in cohort population studies. 


Included in the repository are the following:

- **“Supplementary Table 1.xlsx”** – offers baseline information on the composition of the datasets in this study
- **“Supplementary materials.pdf”** – document enumerating various supplementary materials, tables, and figures that pair with our publication
- **“dX_feature_importance_viz.ipynb”** – Jupyter notebook for generating feature importance plots (individual and compound bar plots) for Dataset X (1, 2, or 3)
- **“dX_feature_importance_viz.html”** – .html file containing feature importance notebook for Dataset X (1, 2, or 3)
- **“dX_ml_pipeline.ipynb”** – Jupyter notebook for running the ML analysis pipeline on Dataset X (1, 2, or 3)
-	**“dX_ml_pipeline.html”** – .html file containing ML analysis pipeline notebook for Dataset X (1, 2, or 3)
-	**“figures.zip”** – zipped folder of .png files containing the original figure files that were generated during analysis
-	**“metric_pub_report.ipynb”** – Jupyter notebook summarizing and comparing performance across models within each dataset (avg./sd, boxplots, and non-parametric statistical comparisons)
-	**“metric_pub_report.html”** – .html file containing metric summary/comparison notebook
-	**“results.zip”** – zipped folder of Excel files containing the raw results (various metrics used) from the ML models in the pipeline for each dataset

*<p align="center">This project was lead by Ryan Urbanowicz and Shannon Lynch of the University of Pennsylvania and the Fox Chase Cancer Center, respectively.</p>*
