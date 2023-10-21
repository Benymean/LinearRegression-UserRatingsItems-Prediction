# Analysis of an E-commerce Dataset: Portfolio Parts 1 & 2

This repository contains a series of analyses on an e-commerce dataset. The analyses span two parts, focusing on understanding user interactions and predicting user ratings for items based on various features.

## Table of Contents

- [Portfolio Part 1](#portfolio-part-1-analysis-of-an-e-commerce-dataset)
  - [Introduction](#introduction)
  - [Description of Fields](#description-of-fields)
  - [Objectives of the Analysis](#objectives-of-the-analysis)
  - [Descriptive Statistics](#descriptive-statistics)
  - [Plotting and Analysis](#plotting-and-analysis)
  - [Boxplot of Helpfulness by Gender](#boxplot-of-helpfulness-by-gender)
- [Portfolio Part 2](#portfolio-part-2-analysis-of-an-e-commerce-dataset)
  - [Introduction](#introduction-1)
  - [Importing the Cleaned E-commerce Dataset](#importing-the-cleaned-e-commerce-dataset)
  - [Dataset Exploration](#dataset-exploration)
  - [Rating's Correlations](#ratings-correlations)
  - [Hypothesis and Observations](#hypothesis-and-observations)
- [Dependencies](#dependencies)
- [License](#license)

---

# Portfolio Part 1: Analysis of an E-commerce Dataset

This repository contains an in-depth analysis of a combined e-commerce dataset. Each user in the dataset has the ability to post a rating and review for the products they purchased. Other users can then evaluate these ratings and reviews, expressing either trust or distrust.

## Table of Contents

1. [Introduction](#introduction)
2. [Description of Fields](#description-of-fields)
3. [Objectives of the Analysis](#objectives-of-the-analysis)
4. [Descriptive Statistics](#descriptive-statistics)
5. [Plotting and Analysis](#plotting-and-analysis)
6. [Boxplot of Helpfulness by Gender](#boxplot-of-helpfulness-by-gender)

## Introduction

The dataset is a rich compilation of e-commerce user information. The dataset offers a comprehensive view of user interactions on an e-commerce platform, from profile details to product reviews. The data is sourced from various platforms and has been merged into a single CSV file named 'A Combined E-commerce Dataset.csv'.

## Description of Fields

- **userId** - The user's ID.
- **gender** - The user's gender.
- **rating** - The user's rating towards the item.
- **review** - The user's review of the item.
- **item** - The item's name.
- **category** - The category of the item.
- **helpfulness** - The average helpfulness of the rating.
- **timestamp** - The timestamp when the rating was created.
- **item_id** - The item's ID.
- **item_price** - The item's price.
- **user_city** - The city of the user's birth.

A user may rate multiple items, and an item may receive ratings and reviews from multiple users. The "helpfulness" metric is an average value based on all the helpfulness values provided by other users.

## Objectives of the Analysis

1. Clean the dataset by removing missing data.
2. Provide descriptive statistics on the cleaned data.
3. Explore correlations and patterns through plotting and analysis.
4. Investigate the relationship between gender and the perceived helpfulness of reviews.

## Descriptive Statistics

Detailed statistical analyses related to the dataset are presented.

## Plotting and Analysis

Visualisations and deeper analyses of the data are presented, exploring correlations and patterns in user behaviour and reviews.

## Boxplot of Helpfulness by Gender

- Both male and female users seem to have reviews with a median helpfulness around 4.
- The range of helpfulness scores is similar for both genders, with scores spread between the lower to upper quartiles.
- There **doesn't seem to be a significant difference** in the perceived helpfulness of reviews based on gender.

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

---

## Dependencies

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## License

MIT License

Copyright (c) 2023 Ben Khalesi

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
