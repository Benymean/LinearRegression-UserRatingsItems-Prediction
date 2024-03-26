# Analysis of an E-commerce Dataset and Predicting User Ratings with Linear Regression

This analysis focuses on training linear regression models to predict users' ratings for items. We explore the impacts of feature selections and varying sizes of training/testing data on model performance.

## Table of Contents

1. [Introduction](#introduction)
2. [Importing the Cleaned E-commerce Dataset](#importing-the-cleaned-e-commerce-dataset)
3. [Dataset Exploration](#dataset-exploration)
4. [Rating's Correlations](#ratings-correlations)
5. [Hypothesis and Observations](#hypothesis-and-observations)

## Introduction

This analysis aims to predict users' ratings for items using linear regression models. This process involves a standard Data Science workflow of data exploration, model training, predictions, and result evaluations. The dataset used is distinct from the one in the initial analysis and is a cleaned combined e-commerce sub-dataset.

## Importing the Cleaned E-commerce Dataset

The dataset, named 'cleaned_ecommerce_dataset.csv', is imported to provide a foundational dataset for our analysis.

## Dataset Exploration

An initial exploration of the dataset offers insights into its structure, number of columns, data types of each column, and more. This step is crucial for understanding the data's characteristics before building prediction models.

## Rating's Correlations

Here, we investigate the correlations between various dataset features like helpfulness, gender, category, review, and the rating. Understanding these correlations is pivotal for creating effective models.

- **Helpfulness:** Correlation coefficient of −0.0075
- **Gender:** Correlation coefficient of -0.0343
- **Category:** Correlation coefficient of -0.1632
- **Review:** Correlation coefficient of −0.0361

## Hypothesis and Observations

From the correlations, the **most correlated feature** with 'rating' is **Category**. It's negatively correlated, suggesting the category might influence the item's rating. The **least correlated feature** is **Helpfulness**, indicating minimal linear relationship with the rating.

---

## Dependencies

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
