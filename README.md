# -Linear-Algebra-Regression-Analysis
Exploring global happiness data and document similarity using linear regression, vector mathematics, and cosine similarity.


📌 Overview

This project applies linear algebra and statistical modeling techniques to analyze two real-world datasets:

World Happiness Report (2018–2019)

Literary text document vectors

The project demonstrates linear regression modeling, statistical inference, and vector similarity analysis.

📂 Datasets
World Happiness Report

Source: Kaggle / World Happiness Report

Years: 2018–2019

Samples: 312 countries

Target Variable: Score

Features include:

GDP per capita

Social support

Life expectancy

Freedom

Generosity

Corruption perception

Text Document Vectors

Source: BloomTech NLP dataset

Documents: 3 literary text segments

Representation: TF / DF weighted vectors

Documents analyzed:

doc0: Pride and Prejudice (Jane Austen)

doc1: Frankenstein (Mary Shelley)

doc2: Frankenstein (Mary Shelley)

🛠️ Tech Stack

Python

pandas

numpy

seaborn

matplotlib

statsmodels

🧪 Project Workflow
Part A: Regression Analysis

Data loading and exploration

Missing value analysis and imputation

Exploratory visualization

Simple linear regression (OLS)

Multiple linear regression

Statistical interpretation

Prediction and residual analysis

Part B: Vector Similarity

Document vector exploration

Dot product and norm calculation

Cosine similarity computation

Author similarity analysis

🧩 Data Preprocessing

Identified and analyzed missing values

Imputed missing corruption scores using median

Verified data types and distributions

Visualized feature relationships

📊 Exploratory Analysis

A seaborn pairplot was used to examine relationships between variables and identify linear trends.

A regression line was visualized between:

GDP per Capita

Happiness Score

📈 Regression Models
Model 1: Simple Linear Regression

Formula:

Score ~ GDP_per_capita


Performance:

R²: 0.637

Slope: 2.25

p-value: < 0.001

Interpretation: GDP per capita explains approximately 64% of the variance in happiness score.

Model 2: Multiple Linear Regression

Formula:

Score ~ GDP_per_capita + Social_support


Performance:

R²: 0.712

Adjusted R²: 0.710

Adding social support improved explanatory power.

📐 Statistical Interpretation

GDP per capita and social support were statistically significant predictors

Both coefficients had p-values < 0.001

95% confidence intervals excluded zero

This confirms strong relationships with happiness score.

🔍 Prediction & Residuals

A prediction was made for Iceland’s happiness score using Model 1.

Example:

Predicted: 6.39  
Observed: 7.50  
Residual: 1.11


This demonstrates practical application of regression outputs.

📏 Cosine Similarity Analysis

Cosine similarity was computed between document vectors:

Pair	Similarity
doc0–doc1	0.130
doc0–doc2	0.099
doc1–doc2	0.322
Interpretation

doc1 and doc2 are most similar

Both were written by Mary Shelley

Cosine similarity correctly identifies common authorship

▶️ How to Run
Clone Repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

Install Dependencies
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels

Launch Notebook
jupyter notebook


Run all cells in the main notebook.

⚠️ Limitations

Small dataset size

Limited predictor variables

Linear model assumptions

Simplified document representation

🌱 Future Improvements

Add interaction terms

Regularized regression

Nonlinear models

Larger text corpora

Word embeddings

👤 Author

Corey Williams BloomTech Data Science Program Sprint 1 - Linear Algebra

LinkedIn: www.linkedin.com/in/ corey-williams-alpha

GitHub: https://github.com/blackbox55


⭐ Why This Project Matters

This project demonstrates:

Applied linear algebra

Statistical modeling

Regression interpretation

Vector similarity methods

Analytical reasoning
