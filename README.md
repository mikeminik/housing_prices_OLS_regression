# Ames Property Prices

The city of Ames, Iowa is interested in assessing property value in an effort to collect information on potential tax revenue. This revenue makes up a significant portion of funding for the city to be put towards essential services and infrastructure. This information will be carried forward into the following fiscal year and incorporated into budgeting considerations. 

Additionally, regular assessment of potential property values can inform decisions on land use and development. It is vital the predictions be as accurate as possible to avoid deficits and unnecessary cuts.

This analysis aims to answer the question: Can we establish a way of predicting fair market value for a collection of properties in Ames, Iowa for the purposes of evaluating upcoming property tax revenue? 

# Data Dictionary

The Ames Property Data Dictionary is extensive and therefore included as an accompanying text file in this project. Refer to Ames Properties Data Dictionary.txt

|File|Description|
|---|---|
|train.csv| This file contains property characteristics in addition to SalePrice, used for training models
|test.csv| This file contains property characteristics without SalePrice, to be used in prediction scoring
|submission1_ols.csv | Predicted sale prices by property Id for homes using the first OLS model
|submission2_ols.csv | Predicted sale prices by property Id for homes using the second, stronger OLS model
|submission3_ridge.csv | Predicted sale prices by property Id for homes using a Ridge cross validated model
|model-ready-data.csv | Tidied data with problematic rows and null values addressed


# Executive Summary

The course of this analysis involved several modeling techniques centered around predicting "Sale Price" which can be interpreted as fair market value of the home. All models were successful at generating predictions, and each were capable of explaining 85% to 88% of the variability in price. 

These results suggest a strong, but not perfect, predictive model. The most likely strongest model was able to predict houses on average within 19,500 dollars while operating on unseen data. This suggests that based on the mill rate of 10.84, the properties provided in the test.csv file would generate property tax revenue of about 1.7M dollars. 


# Areas for further research

- This project was adversely affected by outlier properties, that is to say most often very large houses. Further tuning could harden the model against these properties in the future. 
- This data yield some inferential information on particular characteristics of a house that could be explored further. For example, there were fairly significant correlations to the size of the garage. The city might explore opportunities to encourage citizens to build or remodel these areas to increase market value and in turn, generate more tax revenue. 

## Citations

**Thank you to the following for their involvement in various aspects of the project:**

- Tim Book for instructional material on Python, Pandas, Matplotlib and Seaborn, all of which was used here
- Rowan Schaefer for assistance with handling unseen data and OneHotEncoding
- Emily Rogalski for information on column transformation
- Google Bard for presentation prompt ideas, and for some confirmations on modeling techniques that were chosen


**Sources on external data:**

Kaggle – DSI-910 Ames Housing Challenge  [Online] Available: https://www.kaggle.com/competitions/dsi-910-ames-housing-challenge/data

Iowa Department of Management. "County Property Tax Rates - FY 2010." Accessed October 5, 2023. https://tax.iowa.gov/iowa-tax-rate-history


**Additional thanks to creators and contributors to the following technologies:**

- Python language
- Matplotlib.pyplot library 
- Pandas library
- Numpy library
- Seaborn library
- SciKit-Learn

