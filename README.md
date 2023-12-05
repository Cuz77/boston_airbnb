# Boston Airbnb analysis



## Motivation

This project has been created as a part of the Udacity Nanodegree Data Scientist program. An [article](https://medium.com/@belibels/the-art-of-travel-planning-a-data-driven-approach-e240140fe3b2) has been posted on Medium to share the findings.



## Dependencies

Libraries used for this project:

- pandas
- matplotlib
- sklearn for modeling, testing, and assesing
- wordcloud
- collections



## Summary

This project uses a data-driven approach to optimize travel planning using Airbnb's dataset. We analyzed over 640,000 booking days and 68,000 comments to understand factors influencing accommodation choices. Our analysis revealed that location, apartment standards, and amenities significantly impact price and satisfaction. Interestingly, we found that satisfaction doesn't always correlate with price. We also identified ways to reduce costs without compromising quality by being selective about location and amenities. Our linear model helped identify underpriced areas and unnecessary amenities. This project demonstrates the power of data in making informed travel decisions.



## Structure

The directory structure for this project looks like follows:

    boston_aribnb
    ├── dataset
    │   ├── calendar.csv
    │   ├── listings.csv
    │   ├── reviews.csv
    ├── .gitignore
    ├── boston_airbnb_analysis.ipynb
    └── README.md

- **dataset** folder contains three csv files with the data
- **boston_airbnb_analysis.ipynb** holds the main code for analysis
- **.gitignore** file used mostly to avoid uploading jupiter checkpoints



## Dataset

The dataset consists of three csv files provided by Airbnb on kaggle ([Boston Airbnb Open Data](https://www.kaggle.com/datasets/airbnb/boston/discussion)).
    1. calendar - a list of over 1.3 million bookin days from between 2016-09-06 and 2017-09-05
    2. listings - a list of 3585 airbnb premises
    3. ratings - a list of 68275 ratings with opinions
    


## Data preparation

Categorical variables has been transformed accordingly:
- one-hot encoding has been processed for nominal features
- a feature containing list of available amenities has been transformed into a list of unique values before one-hot encoding
- missing values have been replaced with 0s denoting a lack of option

Numerical variables has been transformed accordingly:
- missing values have been replaced with means
    
    

## Acknowledgements

The image picturing Edgar Allan Poe on the top of the page has been generated by PlusOne, an AI developed by Prosus.

