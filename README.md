# NYC Airbnb Listing Price Prediction

**Authors:** Kien Le, Tony Nguyen  
**Date:** May 25, 2023

## Project Overview

This project analyzes New York City (NYC) Airbnb listing data to predict prices. We utilize the "New York City Airbnb Open Data" dataset from Kaggle, focusing on data cleaning, exploration, and linear regression modeling to gain insights into pricing factors and room type trends.

## Data and Resources Used

We use the "New York City Airbnb Open Data" dataset, which contains information about NYC Airbnb listings. Key variables include:
- `neighbourhood_group`: The borough or area of the listing.
- `room_type`: The type of accommodation.
- `price`: Price per night.
- `minimum_nights`: Minimum stay requirement.
- `number_of_reviews`: Number of reviews.
- `availability_365`: Days available in a year.
- `calculated_host_listings_count`: Host's total listings.

## Data Cleaning and Pre-processing

We perform data cleaning by:
- Checking and handling duplicated values.
- Handling missing values.
- Dropping unnecessary columns.
- Converting columns to factors.
- Removing outliers.

## Linear Regression Model

We build a linear regression model to predict prices based on various features. The model explains a portion of price variability and provides insights into the impact of different factors on pricing.

## Project Structure

- **Data Cleaning**: Code for data cleaning.
- **Data Exploration**: Code for exploring data and generating visualizations.
- **Linear Regression Model**: Code for building and evaluating the linear regression model.

## Usage

To reproduce the analysis, follow these steps:
1. Download the "New York City Airbnb Open Data" dataset from Kaggle.
2. Place the dataset in the project directory and name it "airbnb_data.csv."
3. Run the code in the provided R scripts for data cleaning, exploration, and modeling.

## Conclusion

This project aims to help both hosts and guests make informed decisions about pricing and booking Airbnb accommodations in NYC.

For any questions or further information, contact the authors.
