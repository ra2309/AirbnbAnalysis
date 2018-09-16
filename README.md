# AirbnbAnalysis
Analyzing Airbnb data for Boston and Seattle

### CRISP-DM
Business Understanding:
This data contain a lot of parameters related to Boston and Seattle Airbnb data. Airbnb is in the business of offering host locations for cutomers. Like Amazon, those hosts rely on price and review score. I am assuming that review score correlates with profitability.

Data Understanding:
The data is very dirty but contain a lot of informative insights. So we are required to do a lot of data preprocessing with the data.

Data cleaning and preprocessing:
I spent a lot of time on cleaning the data and you can see from the code that the majority of my work is on data processing. At first, I started by removing columns that are not needed to trim the matrix, then I started remvoing missing data, then removing null data, and then creating dummy variables for categorical columns.

Analysis:
I created a heatmap to show the correlation of data and removed data that are strongly correlated with each other.

Model:
I used a base model which is linear regression which performed poorly. Then, I used decision tree regressor. The model score is 99%.

Deploy:
To deploy this model quickly, we need to neglict calender list since it is huge and rely on the 9 features that we have except host diff. Our model still give 99% accuracy for Boston and Seattle but does not give good results for New York and San Franscisco indicating that each city need its own model and that we need to aggregate data.

### Libraries Used
numpy
pandas
sklearn
pickle
datetime

### Files
Major file is a Notebook for Analyzing airbnb data for Boston and Seattle. It contains the whole process of analyzing to deploying the model.

finalized_model.sav: the decision tree regressor we obtained with all features

deploy_model.sav: model with only 9 features

airbnb_regressor: dot file that shows structure of decision tree regressor
