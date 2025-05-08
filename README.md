# NYC Airbnb Listing Price Prediction (Random Forest Enhanced)

**Authors:** Kien Le, Tony Nguyen  
**Date:** May 25, 2023

## Project Overview

This project analyzes New York City (NYC) Airbnb listing data to predict nightly rental prices. Using the **"New York City Airbnb Open Data"** dataset from Kaggle, we perform comprehensive data cleaning, exploratory analysis, feature engineering, and apply machine learning models—primarily a tuned Random Forest model—to understand and predict Airbnb listing prices more effectively.

## Data and Resources Used

We use the **"New York City Airbnb Open Data"** dataset, which contains rich information about Airbnb listings in NYC. Key variables include:

- `neighbourhood_group`: The borough or area of the listing.
- `room_type`: The type of accommodation.
- `price`: Price per night.
- `minimum_nights`: Minimum stay requirement.
- `number_of_reviews`: Number of reviews.
- `availability_365`: Days available in a year.
- `calculated_host_listings_count`: Host's total listings.
- **Engineered variables** like `review_rate` and `room_borough` were also added.

## Data Cleaning and Pre-processing

We performed rigorous cleaning and transformation steps, including:

- Handling duplicated and missing values.
- Dropping irrelevant columns.
- Converting categorical features into factors.
- Capping extreme price outliers at **$500**.
- Applying a **log transformation** to prices.
- Creating new **interaction-based features**.

## Exploratory Data Analysis

We visualized various aspects of the data including:

- **Price distribution**
- **Room type frequency and their price distributions**
- **Spatial density** of listings by latitude and longitude
- **Borough-level average price** comparisons

These visualizations confirmed the influence of **location and room type** on pricing.

## Machine Learning Model (Random Forest)

We applied a tuned **Random Forest** model with hyperparameters optimized through grid search. Final model settings:

- `mtry = 6`, `nodesize = 5`, `maxnodes = 100`, `ntree = 100`
- **Final performance:** **RMSE = 76.19**, **R² = 0.4365**

## Model Usage Recommendation

This model is best suited for providing **price guidance within common market ranges** (**$50–$250**). It is ideal for:

- Assisting **new hosts** in setting competitive listing prices.
- Enhancing **automated pricing tools** or dashboards.
- Detecting **outliers** in listing prices for quality control.

Due to its averaging nature, the model underperforms on high-end luxury listings and may benefit from **segmentation or follow-up modeling**.

## Project Structure

- **Data Cleaning**: Cleaning, transformation, and feature engineering.
- **Data Exploration**: Visualizations and summary statistics.
- **Modeling**: Hyperparameter tuning, evaluation, and prediction.

## Reproducibility

To reproduce the analysis:

1. Download the **"New York City Airbnb Open Data"** dataset from Kaggle.
2. Save it as `airbnb_data.csv` in your working directory.
3. Run the R Markdown script to reproduce all steps from cleaning to modeling.

## Conclusion

This project delivers a structured, interpretable **machine learning model** that helps predict Airbnb prices in NYC. With approximately **44% of price variance explained**, it offers a solid foundation for further development, especially when enriched with **additional spatial and textual data**.
