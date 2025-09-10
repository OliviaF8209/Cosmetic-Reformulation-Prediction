# Cosmetic Product Reformulation Prediction

## Project Overview

This project explores whether cosmetic products are likely to be reformulated using data from the **California Safe Cosmetics Program (CSCP)**. Reformulations are a critical aspect of the cosmetics industry, often driven by **regulatory changes, safety concerns, or ingredient innovation**.

The goal of this project was to build a **classification model** that predicts if a product will undergo reformulation, and to evaluate the performance of different machine learning approaches.


## Data & Preprocessing

**Dataset:** California Safe Cosmetics Program (CSCP)

* Contains product-level information on cosmetic ingredients, regulatory status, and manufacturer details.

**Preprocessing Steps (not all code included due to space):**

* Data cleaning: removed duplicates, standardized product/ingredient names.
* Feature engineering:

  * **Time-based features** (e.g., time since product introduction).
  * **Regulatory-related features** (e.g., flagged ingredients, chemical categories).
  * **Brand/product-level aggregation** (counts of ingredient classes per product).
* Encoded categorical variables and handled missing values.


## Methods

We compared several models to predict reformulation likelihood:

* Logistic Regression
* Decision Trees
* Random Forest
* XGBoost (primary focus)

**Model Tuning:**

* Hyperparameter optimization (grid search & cross-validation).
* Performance compared across multiple baselines.


## Results

* **XGBoost** outperformed baseline models after including **time-based features**.
* Metrics included:

  * Accuracy
  * Precision, Recall, F1-score
  * Confusion Matrix (see visual below)

*Insert figure of confusion matrix or performance table here*


## Real-World Impact

* Helps manufacturers anticipate when products may require reformulation.
* Supports compliance with regulatory safety standards.
* Demonstrates how **data science + chemistry expertise** can guide decision-making in consumer product development.


## Tools & Libraries

* Python (Pandas, NumPy, scikit-learn, XGBoost)
* Jupyter Notebook
* Matplotlib / Seaborn (visualization)

