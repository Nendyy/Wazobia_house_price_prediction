# Wazobia_house_price_prediction

## Predicting House Prices in Nigeria: A Data Science Project

### Introduction
Real estate is a dynamic market with fluctuating prices influenced by various factors. The goal of this project is to build a predictive model that can help Wazobia Real Estate Limited  in Nigeria determine the optimal pricing for properties based on specific features like location, title, and number of bedrooms, bathrooms and parking space.

### Problem Statement
Predicting house prices in the current market has been a major challenge for Wazobia Real Estate Limited, and they are determined to provide accurate and competitive pricing for houses.

### Aim and Objective
The objective of this project  is to develop a powerful and accurate predictive model that can estimate house prices in Nigeria, and analyse various factors that  impact house prices. 

### Data Access
The dataset used for this project was provided by DSN Network and Zindi Africa for the DSN-MICROSOFT-HACKATHON and can be accessed on the Zindi platform: [Wazobia Real Estate Hackathon Data](https://zindi.africa/competitions/free-ai-classes-in-every-city-hackathon-2023/data).

### Dataset Description
This dataset contains valuable information on various features related to houses, including the location, number of bathrooms, bedrooms, parking spaces, property types, and their corresponding prices.

### Data Preparation
The steps taken in the preparation of this data include:

#### Exploratory Data Analysis 
- Various visualisation charts were used to understand the pattern and behaviour of the dataset. 

#### Data Cleaning 
- Missing values in the 'title' and 'location' columns were imputated with the mode.
- Missing values in the 'bedroom', 'bathroom', and 'parking_space' columns were imputated with their respective median. 
- The 'loc' column was renamed to 'location'.
  
#### Feature Engineering
- created new columns, 'sum_bed_bath_park' and 'ratio_bed_bath'.
- Categorized locations based on population density into 'population_density_level'.
- Encoded 'location' and 'title' columns using TargetEncoder, enhancing model's understanding of location-price and title-price relationship.
 
### Model Building
Various regression algorithms, including Linear Regression, Random Forest, XGBoost, Ridge, Decision Tree, CatBoost, and Support Vector Regression were selected. Linear regression was chosen because it is a simple and interpretable model that can be used for predicting numeric values while Ridge was chosen because of its regularisation abilities. The ensemble methods (Catboost, XGboost, random forest and decision tree) were selected because of their effectiveness in handling complex tasks and ability to capture intricate patterns in the data. Lastly, SVR is selected because of its ability to handle more complex relationships between variables.

### Model Evaluation
The models were evaluated using Root Mean Squared Error (RMSE) to assess their predictive performance.

### Model Selection
The cross validated Catboost regressor model with an rmse of 543,725 was chosen as the model of choice for the prediction because it had the least RMSE score and shows a strong generalisation ability as it performed well on multiple folds of data hence can adapt better to unseen data. 

### Feature Importance Analysis
Feature importance analysis was conducted on the Cross validated Catboost regressor model  to identify which features have the most significant impact on house prices. This analysis provides valuable insights into the factors that drive property prices in Nigeria. The top three features that have significant impact on house prices are The Title, Location, and number of bedrooms. Other contributing features inclde: Population density level, total number of rooms (bedroom, bathroom, parking space), and ratio of bedroom to bathroom. 

### Conclusion 
This data science project successfully predicts house prices for the real estate company based on essential features like location, title, and amenities and the  top-performing model is the Cross-validated Catboost regressor.

### Future Improvements
To enhance the model's performance further, we suggest exploring additional data sources,  adding more features for model training and incorporating more domain knowledge.

### Acknowledgment
I acknowledge the real estate company in Nigeria for providing the dataset and the organisers of the DSN hackathon for hosting this exciting and challenging competition.


