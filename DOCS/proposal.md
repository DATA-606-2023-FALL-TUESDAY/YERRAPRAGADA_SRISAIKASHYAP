
 
## 1. Title and Author

- ### Localized Electric Vehicle Planning
- Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- Sri Sai Kashyap Yerrapragada
- Link to the author's GitHub profile
- [![GitHub Profile](https://img.shields.io/badge/GitHub-Profile-brightgreen.svg)](https://github.com/kyerrapragada)

- Link to the author's LinkedIn progile
- [![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue.svg)](https://www.linkedin.com/in/sri-yerrapragada)

- Link to your PowerPoint presentation file -WIP
- Link to your YouTube video -WIP
    
## 2. Background

Provide the background information about the chosen topic. 

- What is it about?
- The goal of the project is to create a data-driven strategy to encourage and assist the adoption of electric cars while also effectively preparing for the deployment of EV charging infrastructure at the local level. This research attempts to guarantee that infrastructure development corresponds to real adoption patterns by examining previous EV adoption rates and estimating future demand for charging infrastructure based on specific geographic locations (postal codes).

- Why does it matter?
- This project is significant for various reasons:
  Increased EV adoption decreases greenhouse gas emissions and air pollution, resulting in a cleaner environment and lessening the consequences 
   of climate change.
  Energy Sustainability: EV promotion aids in the shift to renewable energy sources, hence improving energy sustainability.
  Economic Advantages: EV adoption boosts the economy by providing employment in the EV sector and reducing reliance on imported fossil fuels.

- What are your research questions?
- What have been the historical trends in electric car adoption rates by Model Year, Make, and Electric car Type in certain geographical locations (postal codes)?

Based on historical data and car characteristics, can we forecast future electric vehicle adoption rates in these areas?

What is the relationship between electric car uptake and expected demand for electric vehicle charging infrastructure at the postal code level?

What are the important takeaways and recommendations for politicians and infrastructure planners to encourage EV adoption and link infrastructure growth with localized demand?

## 3. Data 

Describe the datasets you are using to answer your research questions.

- Data sources
- Data size (MB, GB, etc.)
- Data shape (# of rows and # columns)
- Time period (for example, 2010 to 2020) if your data are time-bound
- **What does each row represent?(a patient, a school, a crime, etc.)**
- Data dictionary
  - Columns name
  - Data type
  - Defition
  - Potential values (for categorical valuables, what are the categories?)
- Which variable/column will be your target/label in your ML model?
- Which variables/columns may be selected as features/predictors for your ML models?

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

