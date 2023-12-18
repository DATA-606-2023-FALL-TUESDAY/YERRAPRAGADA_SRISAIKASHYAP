# 1. Title and Author

- **Project Title:** Prediction of Single-Family Home Price in Texas
- **Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang**
- **Author Name:** Sri Sai Kashyap Yerrapragada
- **Link to the author's GitHub profile:** ![GitHub Logo](https://github.com/DATA-606-2023-FALL-TUESDAY/yerrapragada_srisaikashyap/tree/main)
- **Link to the author's LinkedIn profile:** ![LinkedIn Logo](www.linkedin.com/in/sri-yerrapragada)
- **Link to your PowerPoint presentation file:** [Link to PowerPoint presentation file](https://docs.google.com/presentation/d/16wmJVw65zvD4CAOwVhxow8r1DuR4Z0-8/edit?usp=sharing&ouid=113214851719488513395&rtpof=true&sd=true)

- **Link to your YouTube video:** 
    
# 2. Background

Provide the background information about the chosen topic. 

- **What is it about?** 
  - This study focuses on using machine learning techniques to forecast housing values in the state of Texas. This entails compiling and evaluating a dataset that contains significant variables such as the number of bathrooms, bedrooms, geographical location, and other factors impacting Texas home prices. The objective is to create a machine learning model that can make reliable predictions about property values based on these discovered factors.
- **Why does it matter?** 
  - **Local Market Insight:** Predicting property prices provides buyers, sellers, and real estate professionals with a sophisticated insight.
  - **Educated Decision-Making:** Accurate forecasts enable individuals to make educated decisions, set reasonable expectations, and efficiently navigate the market.
  - Investors gain from recognizing regions with prospective price appreciation, which aids in strategic decisions and portfolio optimization.
  - **Lender Risk Mitigation:** Predictive models assist financial organizations in assessing mortgage lending risks, allowing for better risk management.
  - **Policy Support:** Project findings give significant data for local governments to use in developing housing policies, urban planning plans, and infrastructure development strategies.
- **What are your research questions?**
  - 1. What characteristics have the most influence on forecasting home values in Texas, and how do they contribute to model accuracy?
  - 2. Which machine learning algorithms are most successful in forecasting home values in the Texas real estate market, and how do their accuracy and efficiency compare?
  - 3. Are there geographical differences in the factors impacting home prices among Texas cities or regions, and how may these spatial patterns be incorporated into the prediction model?
  - 4. How have Texas home values evolved over time, and can the forecast model account for temporal phenomena such as seasonality and long-term patterns?
  - 5. What practical insights does the model give for making educated real estate investment decisions, and how can accurate projections of home values effect decision-making for buyers, sellers, and real estate professionals in Texas?

# 3. Data 

- **Data sources:** 
  Data is sourced from [Kaggle - 500,000 US Homes Data for Sale Properties](https://www.kaggle.com/datasets/polartech/500000-us-homes-data-for-sale-properties)

- **Data size:** 
  The dataset is approximately 205 MB in size.

- **Data shape:** 
  The dataset comprises 6,000,000 rows and 28 columns.

- **Time period (if applicable):** 
  The specific time period covered by the data is not mentioned.

- **Row representation:** 
  Each row in the dataset represents a property listing on Zillow.

- **Data dictionary**


| #  | Column              | Dtype   | Definition                                           |
| ---| ------------------- | ------- | ---------------------------------------------------- |
| 0  | property_url        | object  | URL of the property listing                          |
| 1  | property_id         | int64   | Unique identifier for each property                  |
| 2  | address             | object  | Full address of the property                         |
| 3  | street_name         | object  | Name of the street where the property is located     |
| 4  | apartment           | object  | Apartment details if applicable                      |
| 5  | city                | object  | City where the property is located                   |
| 6  | state               | object  | State where the property is located                  |
| 7  | latitude            | float64 | Latitude coordinates of the property                 |
| 8  | longitude           | float64 | Longitude coordinates of the property                |
| 9  | postcode            | object  | Postal code of the property                          |
| 10 | price               | float64 | Price of the property                                |
| 11 | bedroom_number      | float64 | Number of bedrooms in the property                   |
| 12 | bathroom_number     | float64 | Number of bathrooms in the property                  |
| 13 | price_per_unit      | float64 | Price per unit area of the property                  |
| 14 | living_space        | float64 | Living space area of the property                    |
| 15 | land_space          | float64 | Land space area of the property                      |
| 16 | land_space_unit     | object  | Unit of measurement for land space                   |
| 17 | broker_id           | float64 | Unique identifier for the broker (if available)      |
| 18 | property_type       | object  | Type of the property (e.g., house, apartment)        |
| 19 | property_status     | object  | Status of the property (e.g., for sale, sold)        |
| 20 | year_build          | float64 | Year the property was built (if available)           |
| 21 | total_num_units     | float64 | Total number of units in the property (if available) |
| 22 | listing_age         | int64   | Age of the property listing in days                  |
| 23 | RunDate             | object  | Date when the data was recorded                      |
| 24 | agency_name         | object  | Name of the real estate agency (if available)        |
| 25 | agent_name          | float64 | Name of the agent associated with the property       |
| 26 | agent_phone         | float64 | Phone number of the agent (if available)             |
| 27 | is_owned_by_zillow  | int64   | Binary indicator if the property is owned by Zillow  |


- **Target/Label Variable for ML Model:** 
  The target variable for the machine learning model is **price**.

- **Features/Predictors for ML Models:** 
  The following variables/columns are considered as features or predictors for the machine learning models:
  - **bedroom_number**
  - **bathroom_number**
  - **living_space**


# 4. Exploratory Data Analysis (EDA)

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

# 5. Model Training 

- **Predictive Analytics Models:**
  The following models will be employed for predictive analytics:
  - Linear Regression
  - KNN (K-Nearest Neighbors)
  - Random Forest
  - XGBoost
  - Decision Tree

- **Model Training:**
  - **Train vs Test Split:** The dataset will be split into training and testing sets using an 80/20 ratio.
  - **Python Packages:** The models will be implemented using Python packages such as scikit-learn, etc.
  - **Development Environments:** The development environments for model training include your laptop, Google Colab, GitHub CodeSpaces, etc.

- **Performance Measurement and Comparison:**
  The performance of the models will be assessed and compared using relevant evaluation metrics, such as accuracy, precision, recall, and F1 score. Cross-validation techniques may also be employed to ensure robust model evaluation.


# 6. Application of the Trained Models

Develop a web app for people to interact with your trained models. Potential tools for web app development:

- **Streamlit** (recommended for its simplicity and ease to learn)
- Dash
- Flask


# 7. Conclusion

- **Summary of Work and Potential Application:**
  This model aims to predict the price of a single-family home based on the inputs of the number of bedrooms, bathrooms, and the area of living space. The Random Forest model demonstrated superior performance compared to other models.

- **Limitations:**
  While the model shows promise, it has limitations. These may include data constraints, model assumptions, or factors not considered in the current analysis.

- **Lessons Learned:**
  The project provided valuable insights and lessons learned in the fields of machine learning, real estate forecasting, and data analysis.

- **Future Research Directions:**
  - **Feature Enrichment:**
    Exploring the inclusion of new features to enhance forecast accuracy.
  - **Advanced Algorithms:**
    Investigating gradient-boosting strategies to improve overall model performance.
  - **Spatial Analysis:**
    Utilizing spatial analysis to identify location-based factors influencing housing values.
  - **User Interface Enhancement:**
    Implementing a friendly user interface, possibly using Streamlit, for intuitive access and interaction.



# 8. References

- Christopher, A. (2021). *K-Nearest Neighbor: A Deep Dive.* Retrieved from [Link](https://medium.com/swlh/k-nearest-neighbor-ca2593d7a3c4)

- Harode R. (2020). *XGBoost: A Deep Dive into Boosting.* Retrieved from [Link](https://medium.com/sfu-cspmp/xgboost-a-deep-dive-into-boosting-f06c9c41349)

