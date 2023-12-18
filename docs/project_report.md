# The Template and Guideline for the Final Report

- This document serves as a guide for developing project proposal which will eventually become the proposal and final report.
- You start with the end in mind and adopt an agile approach:
  - Making progress continuously towards your goal.
  - Updating this document continuously along the way.
 
## 1. Title and Author

- Project Title: Prediction of Single-Family Home Price in Texas
- Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- Author Name : Sri Sai Kashyap Yerrapragada
- Link to the author's GitHub profile: ![GitHub Logo](https://github.com/DATA-606-2023-FALL-TUESDAY/yerrapragada_srisaikashyap/tree/main)
- Link to the author's LinkedIn profile: ![LinkedIn Logo](www.linkedin.com/in/sri-yerrapragada)
- Link to your PowerPoint presentation file: (https://docs.google.com/presentation/d/16wmJVw65zvD4CAOwVhxow8r1DuR4Z0-8/edit?usp=sharing&ouid=113214851719488513395&rtpof=true&sd=true)
- Link to your YouTube video: 
    
## 2. Background

Provide the background information about the chosen topic. 

- What is it about? 
- This study focuses on using machine learning techniques to forecast housing values in the state of Texas. This entails compiling and evaluating a dataset that contains significant variables such as the number of bathrooms, bedrooms, geographical location, and other factors impacting Texas home prices. The objective is to create a machine learning model that can make reliable predictions about property values based on these discovered factors.
- Why does it matter? 
- Local Market Insight: Predicting property prices provides buyers, sellers, and real estate professionals with a sophisticated insight.

educated Decision-Making: Accurate forecasts enable individuals to make educated decisions, set reasonable expectations, and efficiently navigate the market.

- Investors gain from recognizing regions with prospective price appreciation, which aids in strategic decisions and portfolio optimization.

Lender Risk Mitigation: Predictive models assist financial organizations in assessing mortgage lending risks, allowing for better risk management.

Policy Support: Project findings give significant data for local governments to use in developing housing policies, urban planning plans, and infrastructure development strategies.

- What are your research questions?
- 1. What characteristics have the most influence on forecasting home values in Texas, and how do they contribute to model accuracy?

2. Which machine learning algorithms are most successful in forecasting home values in the Texas real estate market, and how do their accuracy and efficiency compare?

3. Are there geographical differences in the factors impacting home prices among Texas cities or regions, and how may these spatial patterns be incorporated into the prediction model?

4. How have Texas home values evolved over time, and can the forecast model account for temporal phenomena such as seasonality and long-term patterns?

5. What practical insights does the model give for making educated real estate investment decisions, and how can accurate projections of home values effect decision-making for buyers, sellers, and real estate professionals in Texas?

- 

## 3. Data 

Describe the datasets you are using to answer your research questions.

- Data sources: Data is sourced from [https://www.kaggle.com/datasets/polartech/500000-us-homes-data-for-sale-properties](https://www.kaggle.com/datasets/polartech/500000-us-homes-data-for-sale-properties)

- Data size (MB, GB, etc.): Size of the data is 205 MB
- Data shape (# of rows and # columns): (6000000,28)
- Time period (for example, 2010 to 2020) if your data are time-bound
- **What does each row represent?(a patient, a school, a crime, etc.)**: Each row of data represents a property listing in Zillow
- Data dictionary
  - Columns name
  - Data type
  - Defition
  - Potential values (for categorical valuables, what are the categories?)
| #   | Column             | Dtype   | Definition                                           |
| --- | ------------------ | ------- | ---------------------------------------------------- |
| 0   | property_url       | object  | URL of the property listing                          |
| 1   | property_id        | int64   | Unique identifier for each property                  |
| 2   | address            | object  | Full address of the property                         |
| 3   | street_name        | object  | Name of the street where the property is located     |
| 4   | apartment          | object  | Apartment details if applicable                      |
| 5   | city               | object  | City where the property is located                   |
| 6   | state              | object  | State where the property is located                  |
| 7   | latitude           | float64 | Latitude coordinates of the property                 |
| 8   | longitude          | float64 | Longitude coordinates of the property                |
| 9   | postcode           | object  | Postal code of the property                          |
| 10  | price              | float64 | Price of the property                                |
| 11  | bedroom_number     | float64 | Number of bedrooms in the property                   |
| 12  | bathroom_number    | float64 | Number of bathrooms in the property                  |
| 13  | price_per_unit     | float64 | Price per unit area of the property                  |
| 14  | living_space       | float64 | Living space area of the property                    |
| 15  | land_space         | float64 | Land space area of the property                      |
| 16  | land_space_unit    | object  | Unit of measurement for land space                   |
| 17  | broker_id          | float64 | Unique identifier for the broker (if available)      |
| 18  | property_type      | object  | Type of the property (e.g., house, apartment)        |
| 19  | property_status    | object  | Status of the property (e.g., for sale, sold)        |
| 20  | year_build         | float64 | Year the property was built (if available)           |
| 21  | total_num_units    | float64 | Total number of units in the property (if available) |
| 22  | listing_age        | int64   | Age of the property listing in days                  |
| 23  | RunDate            | object  | Date when the data was recorded                      |
| 24  | agency_name        | object  | Name of the real estate agency (if available)        |
| 25  | agent_name         | float64 | Name of the agent associated with the property       |
| 26  | agent_phone        | float64 | Phone number of the agent (if available)             |
| 27  | is_owned_by_zillow | int64   | Binary indicator if the property is owned by Zillow  |

- Which variable/column will be your target/label in your ML model? price
- Which variables/columns may be selected as features/predictors for your ML models? bedroom_number, bathroom_number, living_space

## 4. Exploratory Data Analysis (EDA)

- Perform data exploration using Jupyter Notebook
- You would focus on the target variable and the selected features and drop all other columns.
- produce summary statistics of key variables
- Create visualizations (I recommend using **Plotly Express**)
- Find out if the data require cleansing:
  - Missing values?
  - Duplicate rows? 
- Find out if the data require splitting, merging, pivoting, melting, etc.
- Find out if you need to bring in other data sources to augment your data.
  - For example, population, socioeconomic data from Census may be helpful.
- For textual data, you will pre-process (normalize, remove stopwords, tokenize) them before you can analyze them in predictive analysis/machine learning.
- Make sure the resulting dataset need to be "tidy":
  - each row represent one observation (ideally one unique entity/subject).
  - each columm represents one unique property of that entity. 

## 5. Model Training 

- What models you will be using for predictive analytics?
- Models used: Linear Regression, KNN, Random Forest, XGBoost, Decision Tree
- How will you train the models?
  - Train vs test split (80/20, 70/30, etc.): Train vs Split ration is 80/20
  - Python packages to be used (scikit-learn, NLTK, spaCy, etc.) 
  - The development environments (your laptop, Google CoLab, GitHub CodeSpaces, etc.)
- How will you measure and compare the performance of the models?

## 6. Application of the Trained Models

Develop a web app for people to interact with your trained models. Potential tools for web app development:

- **Streamlit** (recommended for its simplicity and ease to learn)
- Dash
- Flask

## 7. Conclusion

- Summarize your work and its potetial application
- This model predicts the price of a single-family home based on the inputs of number of bedrooms, bathrooms, and area of living space. 
Random Forest performed better as compared to the other models.  

- Point out the limitations of your work
- Lessons learned 
- Talk about future research direction
- Feature enrichment: Including new features to improve forecast accuracy.
Advanced algorithms: Investigating gradient-boosting strategies for better model performance.
Spatial analysis: Using spatial analysis to identify location-based factors that influence housing values.
Friendly user interface: Using Streamlit to create an intuitive user interface for simple access and interaction.



## 8. References 

List articles, blogs, and websites that you have referenced or used in your project.