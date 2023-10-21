# Portfolio Part 2: Analysis of an E-commerce Dataset

Continuing from "Analysis of an E-commerce Dataset", this analysis focuses on training linear regression models to predict users' ratings for items. We explore the impacts of feature selections and varying sizes of training/testing data on model performance.

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

## Dependencies

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
---

## License

MIT License

Copyright (c) 2023 Ben Khalesi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
