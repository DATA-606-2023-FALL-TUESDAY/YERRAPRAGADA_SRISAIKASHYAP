
 
## 1. Title and Author

# **Localized Electric Vehicle Planning**

*Prepared for UMBC Data Science Master Degree Capstone by Dr. Chaojie (Jay) Wang*

**Author Name:** Sri Sai Kashyap Yerrapragada

- [GitHub Profile](https://github.com/kyerrapragada)
- [LinkedIn Profile](https://www.linkedin.com/in/sri-yerrapragada)
- [Link to PowerPoint presentation file (_Work in Progress_)](link-to-ppt-file)
- [Link to YouTube video (_Work in Progress_)](link-to-youtube-video)

    
## 2. Background

**What is it about?**

The goal of the project is to create a data-driven strategy to encourage and assist the adoption of electric cars while also effectively preparing for the deployment of EV charging infrastructure at the local level. This research attempts to guarantee that infrastructure development corresponds to real adoption patterns by examining previous EV adoption rates and estimating future demand for charging infrastructure based on specific geographic locations (postal codes).

**Why does it matter?**

This project is significant for various reasons:

- Increased EV adoption decreases greenhouse gas emissions and air pollution, resulting in a cleaner environment and lessening the consequences of climate change.
- Energy Sustainability: EV promotion aids in the shift to renewable energy sources, hence improving energy sustainability.
- Economic Advantages: EV adoption boosts the economy by providing employment in the EV sector and reducing reliance on imported fossil fuels.

**Research questions:**

1. What have been the historical trends in electric car adoption rates by Model Year, Make, and Electric car Type in certain geographical locations (postal codes)?
2. Based on historical data and car characteristics, can we forecast future electric vehicle adoption rates in these areas?
3. What is the relationship between electric car uptake and expected demand for electric vehicle charging infrastructure at the postal code level?
4. What are the important takeaways and recommendations for politicians and infrastructure planners to encourage EV adoption and link infrastructure growth with localized demand?


## 3. Data 

**Data Sources:**

- Data is sourced from [Data.gov - Electric Vehicle Population Data](https://catalog.data.gov/dataset/electric-vehicle-population-data).

**Data Details:**

- Data Size: 113.17 MB

- Data Shape: (143596,17)

- Time Period: 1997-2004


Each row in the dataset represents a registered electric vehicle in Washington state.

**Data Dictionary:**

|   # | Column Name                                      | Data Type |  Definition  |  Potential Values  |
|    # | Column                | Definition                                                | Dtype   | Potential Values |
| ---: | :-------------------- | :-------------------------------------------------------- | :------ | :--------------- |
|    0 | VIN (1-10)            | Vehicle Identification Number (characters 1-10)           | object  |
|    1 | County                | County where the vehicle is registered                    | object  |
|    2 | City                  | City where the vehicle is registered                      | object  |
|    3 | State                 | State where the vehicle is registered                     | object  |
|    4 | Postal Code           | Postal code of the registration location                  | float64 |
|    5 | Model Year            | Year of the vehicle's model                               | int64   |
|    6 | Make                  | Manufacturer or make of the vehicle                       | object  |
|    7 | Model                 | Model name or number of the vehicle                       | object  |
|    8 | Electric Vehicle Type | Type of electric vehicle (e.g., Hybrid, Plug-in Electric) | object  |
|    9 | CAFV Eligibility      | Clean Alternative Fuel Vehicle (CAFV) Eligibility         | object  |
|   10 | Electric Range        | Electric range of the vehicle (in miles)                  | int64   |
|   11 | Base MSRP             | Manufacturer's suggested retail price (in USD)            | int64   |
|   12 | Legislative District  | Legislative district where the vehicle is registered      | float64 |
|   13 | DOL Vehicle ID        | Department of Licensing (DOL) Vehicle ID                  | int64   |
|   14 | Vehicle Location      | Location of the vehicle                                   | object  |
|   15 | Electric Utility      | Electric utility provider for the vehicle                 | object  |
|   16 | 2020 Census Tract     | Census tract of the registration location                 | float64 |





**Target/Label Variable:** 

**Feature/Predictor Variables:** 


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
- How will you train the models?
  - Train vs test split (80/20, 70/30, etc.)
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
- Point out the limitations of your work
- Lessons learned 
- Talk about future research direction

## 8. References 

List articles, blogs, and websites that you have referenced or used in your project.

