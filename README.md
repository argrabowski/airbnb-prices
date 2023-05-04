# Machine Learning to Predict Airbnb Listing Prices

## Overview and Motivation

This report describes a machine learning project to predict the price of Airbnb listings in Boston using various techniques such as data cleaning, feature engineering, and model selection. Different algorithms, including linear regression and gradient boosting, were used and evaluated using performance metrics. The project also involved hypothesis testing and the findings suggest that the model can accurately predict listing prices, which can be beneficial for hosts and policymakers. The project aims to provide a better understanding of the Boston Airbnb market and can potentially inform policymakers in their efforts to regulate the short-term rental market while allowing hosts to optimize their pricing strategy and prospective tenants to determine the value of a listing.

## Research Aims

The project aims to develop a regression model that can predict the price of Airbnb listings in Boston with an 80% accuracy rate. The research question is focused on whether the model can effectively determine if a listing's price is reasonable for both listing and purchasing by considering various characteristics like location, amenities, and number of rooms. The predictor variables of the highest performing model include attributes such as bedrooms, host acceptance rate, and latitude. The null hypothesis states that the model cannot predict the price of a listing with 80% accuracy, while the alternative hypothesis suggests that it can.

## Dataset

The dataset used in this project is Inside Airbnb's Boston, MA dataset, which includes information on Airbnb listings in Boston, MA, such as location, price, and number of bedrooms and bathrooms. The dataset is updated quarterly and contains information on 3,703 listings made during the fourth quarter of 2022. While the dataset is valuable, it is self-reported by hosts and only spans a quarter-year. The data was cleaned and feature engineering was performed, including creating a list of selected amenities and new columns indicating their presence and count per listing.

## Exploratory Data Analysis

The exploratory data analysis phase involved creating various visualizations such as pie charts, histograms, box plots, scatter plots, heatmaps, and violin plots to understand the data and the relationship between attributes. The correlation between categorical and numerical attributes, and the correlation of the attributes with the response variable (price) were also calculated. Feature engineering was done by encoding categorical attributes and scaling numerical attributes. The top thirty attributes with the highest correlations were chosen, and redundant columns were removed while new columns were created for selected amenities. The EDA phase was crucial in gaining a more profound understanding of the data and selecting the most relevant attributes for the final dataset.

![](/src/images/vis_one.png)

## Final Analysis

This project aimed to predict Airbnb listing prices using seven different regression models and evaluate their performance using MSE, MAE, and R-squared. Gradient boosting and K-nearest neighbor were the best performing models, while decision tree and multi-layer perceptron regression performed poorly. Hyperparameters were tuned using grid search and cross-validation for K-nearest neighbor, random forest, and gradient boosting models. The study demonstrated the significant impact of the choice of model and hyperparameters on the prediction accuracy. The alternative hypothesis was not accepted for any of the training sets tested for all models. Overall, testing various regression models and tuning their hyperparameters led to a more accurate prediction of Airbnb listing prices.

![](/src/images/model_sel.png)

## Conclusion

This project developed a machine learning model to predict Airbnb listing prices in Boston based on various attributes, achieving an R-squared score of 0.60. The gradient boosting regressor outperformed all other models. Feature engineering, including encoding categorical attributes and scaling numerical attributes, and selecting the top thirty attributes with the highest correlations, enhanced the model's performance. The model offers valuable insights for hosts and policymakers, and the project explored the most significant features affecting listing price and neighborhood pricing. Future research directions include examining the impact of essential amenities on listing prices.
