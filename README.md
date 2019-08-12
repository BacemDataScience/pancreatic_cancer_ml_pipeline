# pancreatic_cancer_ml_pipeline

This study is an exploration of various machine learning models (and the statistical comparison of these models) as they apply to patient health data with varying degrees and types of bias. The three datasets utilized in this analysis were obtained from the Prostrate, Lung, Colorectal, and Ovarian (PLCO) Cancer Trial; in this study, we work with pancreatic cancer data obtained as a corollary from the trial. The datasets each included health records for both cases (patients who had pancreatic cancer) and controls (patients who did not have pancreatic cancer).

The primary research objectives of this study are to develop a comprehensive machine learning pipeline encompassing a broad spectrum of models to be compared across datasets, as well as to assess various contributors of bias between datasets and how they can be handled in machine learning population-based cohort studies. 

This repository contains the Jupyter notebooks, and supplemental materials for our research paper on assessing machine learning bias in cohort population studies. 


Included in the repository are the following:

- **"Pipeline.png"** - figure containing the basic structure of the ML analysis pipeline that was implemented
- **“Supplementary Table 1.xlsx”** – offers baseline information on the composition of the datasets in this study
- **“Supplementary materials.pdf”** – document enumerating various supplementary materials, tables, and figures that pair with our publication
- **“dX_feature_importance_viz.ipynb”** – Jupyter notebook for generating feature importance plots (individual and compound bar plots) for Dataset X (1, 2, or 3); also available as an html file
- **“dX_ml_pipeline.ipynb”** – Jupyter notebook for running the ML analysis pipeline on Dataset X (1, 2, or 3); also available as an html file
-	**“figures.zip”** – zipped folder of .png files containing the original figure files that were generated during analysis
-	**“metric_pub_report.ipynb”** – Jupyter notebook summarizing and comparing performance across models within each dataset (avg./sd, boxplots, and non-parametric statistical comparisons); also available as an html file
-	**“results.zip”** – zipped folder of Excel files containing the raw results (various metrics used) from the ML models in the pipeline for each dataset

The same general framework was implemented for the pipeline of each dataset (see figure below).

![Alt text](Pipeline.png)

For each dataset, the data was first partitioned into 10 cross-validation training and testing datasets. Each of these 10 training sets underwent feature selection (MultiSURF and mutual information algorithms were implemented) in order to identify and filter out the most important features to be included in the analysis. Following this, the hyperparameters were tuned for each model and training set. These optimal hyperparameters were then fed into their respective models and used to train the training dataset for which they were optimized. Lastly, the testing dataset corresponding to each training dataset was used to test each trained model and obtain various classification metrics on which to evaluate and compare the models.

*<p align="center">This project was led by **Ryan Urbanowicz** and **Shannon Lynch** of the University of Pennsylvania and the Fox Chase Cancer Center, respectively.</p>*
*<p align="center">**Pranshu Suri** and **Yuhan Cui**, of the University of Pennsylvania, were contributors to assembling this pipeline.</p>*
