# Diabetes Prediction Analysis

[![View Analysis Website](https://img.shields.io/badge/View-Analysis%20Website-blue)](https://yanting322.github.io/diabetes-prediction-analysis/)

This project presents a comprehensive exploratory data analysis and machine learning approach for predicting diabetes using patient health records. The analysis includes data cleaning, feature engineering, visualization, and model training using Random Forest with robust handling of class imbalance (SMOTE & undersampling).

**🔗 [Analysis Website](https://yanting322.github.io/diabetes-prediction-analysis/)**  
> Explore the full analysis, feature importance, and visualizations online.

---

## Project Structure

- `Analysis.ipynb`: Main Jupyter Notebook (analysis, modeling, plots)
- `diabetes_prediction_dataset.csv`: Source dataset
- `index.qmd`: Quarto homepage redirect
- `about.qmd`: About page
- `docs/` (rendered HTML site for GitHub Pages)
    - `index.html`
    - `Analysis.html`
    - ... (site assets, CSS, etc.)
- `_quarto.yml`: Quarto site configuration
- `README.md`: Project introduction and usage

## Analysis Workflow

- **Data Cleaning & Preprocessing**  
    - Handle missing values, outliers, and categorical encoding (including one-hot encoding for correlation/visualization).

- **Exploratory Data Analysis**
    - Distribution of features (age, gender, BMI, smoking history, etc.)
    - Relationship between features and diabetes occurrence (bar plots, box plots, violin plots)

- **Feature Engineering**
    - Removal of irrelevant categories (e.g., ‘Other’ gender)
    - Outlier filtering (e.g., BMI > 60)
    - Encoding for machine learning and correlation analysis

- **Handling Imbalanced Data**  
  Combined oversampling (SMOTE) and undersampling strategies in the training pipeline.

- **Modeling**
    - Random Forest classifier with hyperparameter tuning via GridSearchCV and cross-validation
    - Robust evaluation on validation and test sets, with no resampling applied to validation/test (for real-world simulation)

- **Feature Importance**  
  Quantitative ranking of features’ predictive power.

- **Result Visualization**
    - Correlation heatmaps, importance plots, and more

## How to Reproduce
- **Environment:**
Install dependencies (Python 3.8+ recommended).
  - scikit-learn
	-	imbalanced-learn
	-	matplotlib, seaborn, pandas, numpy
	-	quarto (for site generation)
- **Run the Analysis:**
Open Analysis.ipynb and execute all cells.
- **Build the Website:**
  -	Install Quarto
	-	Render locally with:
