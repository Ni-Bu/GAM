# Generalized Additive Models (GAMs) for Airbnb Price Prediction

## Project Overview

This project implements Generalized Additive Models (GAMs) to predict Airbnb listing prices in New York City. We explore different basis functions (spline, polynomial, and step function) and compare their performance against a linear regression baseline. The project demonstrates the interpretability of GAMs through partial dependence plots.

Note: Detailed explanations, analysis, and interpretations are primarily contained within the Jupyter notebook itself.

## Dataset

We use the ["New York City Airbnb Open Data"](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data) dataset from Kaggle:

-   File: `AB_NYC_2019.csv`
-   Features used: latitude, longitude, minimum_nights, number_of_reviews, reviews_per_month, calculated_host_listings_count, availability_365
-   Target variable: price

## Installation

1. Ensure you have Python 3.7+ installed.
2. Install required libraries:
    ```
    pip install pandas numpy scikit-learn pygam matplotlib
    ```

## Project Structure

-   `assignment1.ipynb`: Jupyter notebook containing all code and analysis
-   `README.md`: This file
-   `AB_NYC_2019.csv`: Dataset file (not included in the repository)

## Usage

1. Open `assignment1.ipynb` in Jupyter Notebook or VS Code with Jupyter extension.
2. Ensure `AB_NYC_2019.csv` is in the same directory.
3. Run all cells in the notebook sequentially.

## Implementation Details

1. Data Preprocessing:

    - Feature selection
    - Handling missing values
    - Scaling features

2. Models Implemented:

    - Linear Regression (baseline)
    - GAM with spline basis
    - GAM with polynomial basis
    - GAM with step function basis (approximated using splines)

3. Visualization:
    - Partial dependence plots for each feature in all GAM models
    - Rug plots to show data distribution
    - R-squared comparison bar plot

## Interpreting Partial Dependence Plots

-   X-axis: Feature values
-   Y-axis: Partial effect on predicted price
-   Blue line: Estimated partial dependence function
-   Red dotted lines: Confidence intervals

## Acknowledgments

-   Kaggle for providing the dataset
-   pygam library developers
-   Generative AI for the documentation
