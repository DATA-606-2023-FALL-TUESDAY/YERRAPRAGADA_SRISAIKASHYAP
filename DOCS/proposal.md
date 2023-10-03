## 1. Title and Author

# **Real Estate Price Analysis and Prediction**

*Prepared for UMBC Data Science Master Degree Capstone by Dr. Chaojie (Jay) Wang*

**Author Name:** Sri Sai Kashyap Yerrapragada

- [GitHub Profile](https://github.com/kyerrapragada)
- [LinkedIn Profile](https://www.linkedin.com/in/sri-yerrapragada)
- [Link to PowerPoint presentation file (_Work in Progress_)](link-to-ppt-file)
- [Link to YouTube video (_Work in Progress_)](link-to-youtube-video)

    
## 2. Background

**What is it about?**

The goal of this project is to develop a data-driven approach for predicting real estate prices and providing valuable insights into the housing market. This research aims to leverage a dataset containing property information, such as location, price, bedroom and bathroom counts, living space, to build predictive models and facilitate informed decision-making in the real estate industry.

**Why does it matter?**

This project holds significance for several reasons:

- Informed Investment: Accurate price predictions assist potential buyers, sellers, and investors in making informed real estate decisions.
- Market Insights: Analyzing real estate data provides insights into market trends, helping professionals adapt to changing conditions.
- Economic Impact: The housing market has a substantial impact on the economy, and informed decisions can contribute to economic stability.

**Research questions:**

1. How can we predict real estate prices based on property features such as location, size, and etc?
2. What are the key factors influencing property prices, and how do they vary by location (postcode)?
3. Can machine learning models provide valuable insights into property market dynamics?
4. How can the results of this analysis benefit real estate professionals and individuals interested in property investment?


## 3. Data 

**Data Sources:**

- Data is sourced from [Kaggle Datasets- 500000+ US Homes Data](https://www.kaggle.com/datasets/polartech/500000-us-homes-data-for-sale-properties).

**Data Details:**

- Data Size: 128.2 MB
- Data Shape: (600000,25)

Each row in the dataset represents a property listing.

**Data Dictionary:**

|    # | Column             | Definition                                         | Dtype   | Potential Values |
| ---: | :----------------- | :------------------------------------------------- | :------ | :--------------- |
|    0 | property_id        | Unique identifier for each property listing        | int64   |                  |
|    1 | address            | Address of the property                            | object  |                  |
|    2 | city               | City where the property is located                 | object  |                  |
|    3 | state              | State where the property is located                | object  |                  |
|    4 | latitude           | Latitude coordinate of the property                | float64 |                  |
|    5 | longitude          | Longitude coordinate of the property               | float64 |                  |
|    6 | postcode           | Postal code of the property                        | object  |                  |
|    7 | price              | Price of the property (target variable)            | float64 |                  |
|    8 | bedroom_number     | Number of bedrooms in the property                 | float64 |                  |
|    9 | bathroom_number    | Number of bathrooms in the property                | float64 |                  |
|   10 | price_per_unit     | Price per unit area of the property                | float64 |                  |
|   11 | living_space       | Living space area of the property (in sq. ft.)     | float64 |                  |
|   12 | land_space         | Land space area of the property                    | float64 |                  |
|   13 | land_space_unit    | Unit of measurement for land space (e.g., sq. ft.) | object  |                  |
|   14 | broker_id          | Broker identifier (no values present)              | float64 |                  |
|   15 | property_type      | Type of property (e.g., residential, commercial)   | object  |                  |
|   16 | property_status    | Status of the property listing                     | object  |                  |
|   17 | year_build         | Year the property was built (no values present)    | float64 |                  |
|   18 | total_num_units    | Total number of units (no values present)          | float64 |                  |
|   19 | listing_age        | Age of the property listing (in years)             | int64   |                  |
|   20 | RunDate            | Date of the data run                               | object  |                  |
|   21 | agency_name        | Name of the agency associated with the property    | object  |                  |
|   22 | agent_name         | Agent's name (no values present)                   | float64 |                  |
|   23 | agent_phone        | Agent's phone number (no values present)           | float64 |                  |
|   24 | is_owned_by_zillow | Binary indicator if owned by Zillow (0 or 1)       | int64   | 0 (No), 1 (Yes)  |



**Target/Label Variable:** price

**Feature/Predictor Variables:** postcode, city, bedroom_number, bathroom_number, living_space


## 4. Exploratory Data Analysis (EDA)

- Perform data exploration using Jupyter Notebook
- Focus on the target variable (Price) and selected features
- Calculate summary statistics of key variables
- Create visualizations, utilizing tools like **Matplotlib** and **Seaborn**
- Check for data quality issues:
  - Missing values
  - Duplicate rows
- Assess the need for data preprocessing or augmentation, such as incorporating demographic data from census sources.

## 5. Model Training 

- Utilize machine learning models for real estate price prediction
- Split the dataset into training and testing sets (e.g., 80/20)
- Python packages for modeling (e.g., scikit-learn)
- Measure and compare model performance using appropriate metrics (e.g., RMSE, MAE, R-squared)

## 6. Application of the Trained Models

Develop a web application to enable users to interact with the trained models and obtain property price predictions. Recommended tools for web app development:

- **Streamlit** (recommended for its simplicity and ease of use)
- Dash
- Flask

## 7. Conclusion

- Summarize the project's objectives and outcomes
- Highlight the potential applications of the predictive models in the real estate industry
- Discuss project limitations and lessons learned
- Suggest directions for future research in real estate analytics

## 8. References 

List articles, blogs, datasets, and other resources that you have referenced or used in your project.
