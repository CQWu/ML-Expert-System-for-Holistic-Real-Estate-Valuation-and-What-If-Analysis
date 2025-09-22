# ML Expert System for Real Estate Valuation and What-If Analysis

This repository contains the supporting data files, notebooks, and inference results for the study: **"ML Expert System for Real Estate Valuation and What-If Analysis."**

Our goal with this project was to develop a machine learning-based system capable of accurately valuing real estate properties and performing "what-if" analysis to understand the impact of various features on property prices.

**Please note:** The core expert system files are proprietary and are not included in this public repository.

---

## Repository Contents

This repository provides a complete pipeline from raw data to modeling and inference. Below is a detailed breakdown of the key files and directories.

### `/data/`

This directory contains the datasets used for the project.

* `kc_house_data.csv`: The **original raw dataset** containing house sale prices for King County, WA.
    * *Source*: [House Sales in King County, USA on Kaggle](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)
* `zipcode_info.csv`: **Additional zipcode-based features** (e.g., population density, median income) that were scraped from the web to enrich the original dataset.
* `data3_0505.csv`: The **final, preprocessed dataset** that is the result of the data cleaning and feature engineering process. This file is used for all modeling.

### `/notebooks/`

This directory includes all the Jupyter notebooks used for the analysis.

* `ML_Real_Estate_Expert_System_Data_Preprocessing.ipynb`: The notebook for all **data preprocessing steps**. It takes the raw data, merges it with supplementary info, and performs cleaning and feature engineering to produce `data3_0505.csv`.
* `ML_Real_Estate_Expert_System_Base_Models_Part1.ipynb`, `Part2.ipynb`, and `Part3.ipynb`: Notebooks for training and evaluating a variety of **base machine learning models**, such as K-Nearest Neighbors (KNN), Decision Trees, Random Forest, Support Vector Machines (SVM), and more.
* `ML_Real_Estate_Expert_System_Stacking_Model.ipynb`: The notebook where the predictions from the base models are combined using a **stacking ensemble model** to improve valuation accuracy.
* `ML_Real_Estate_Expert_System_Inference.ipynb`: The notebook used for **causal inference and what-if analysis**. It estimates the financial impact of changing a single property feature (e.g., improving the 'condition' or 'view') on the final sale price.

### `/results/`

This directory stores the output files from the inference analysis.

* `condition.csv`, `view.csv`, etc.: CSV files containing the **inference results**. Each file shows the estimated effect of a specific factor on property values.

---

## Citation

[Name Place Holder]. (2025). ML Expert System for Holistic Real-Estate Valuation and What-If Analysis (Version 1.0) [Computer software]. GitHub. https://github.com/CQWu/ML-Expert-System-for-Holistic-Real-Estate-Valuation-and-What-If-Analysis
