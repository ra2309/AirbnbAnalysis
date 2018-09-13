# AirbnbAnalysis
Analyzing Airbnb data for Boston and Seattle

Business Understanding:
This data contain a lot of parameters related to Boston and Seattle Airbnb data. Airbnb is in the business of offering host locations for cutomers. Like Amazon, those hosts rely on price and review score. I am assuming that review score correlates with profitability.

Data Understanding:
The data is very dirty but contain a lot of informative insights. So we are required to do a lot of data preprocessing with the data.

Data cleaning and preprocessing:
I spent a lot of time on cleaning the data and you can see from the code that the majority of my work is on data processing. At first, I started by removing columns that are not needed to trim the matrix, then I started remvoing missing data, then removing null data, and then creating dummy variables for categorical columns.

Analysis:
I created a heatmap to show the correlation of data and removed data that are strongly correlated with each other.

Model:
I used a base model which is linear regression which performed poorly. Then, I took the best 10 features using univariate select k best chi2 and used decission tree. The model score is 99%.
