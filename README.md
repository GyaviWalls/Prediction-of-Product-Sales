# Prediction-of-Product-Sales

### Ayebare Gyavira

"Never make a trade or take an action unless it's backed by reason and analysis." - William J. O'Neil

In attempt to maximise profits, salesmen are required to maximise their sales as one of the means to achieve their goal. But sometimes sales vary due to randomised factors. Predicting them is one of the solutions that could be employed to understand that chaos and use it to your advantage. In this project, we look at the procedures taken to understand the data present and how it can be used to increase sales

### Data Source:

Sales Predictions 2023 [https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view?usp=sharing](https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view?usp=sharing)

In the original dataset, there werer 8523 rows and 12 columns.

### Data Dictionary

<img width="749" alt="data_dictionary" src="https://github.com/GyaviWalls/Prediction-of-Product-Sales/assets/44253554/599c0377-b025-4b56-a289-9300c8f5ab18">


To prepare this data, the data was cleaned, and the following processes were performed:

### Exploratory Data Analysis

- To visualize the data for explantory purposes, a bargraph and a heatmap were chosen.
- The bargraph was chosen to show how the number of sold item types compare to each other. 
- The heatmap was chosen to show the degree of correlation that the numeric features had with each other. 

![aim](https://github.com/GyaviWalls/Prediction-of-Product-Sales/assets/44253554/fca01d5e-4c8b-44fa-b163-2e17a592fb36)


This histogram shows that the cheaper an item is, the more its sold.


![heatmap](https://github.com/GyaviWalls/Prediction-of-Product-Sales/assets/44253554/000cf39f-502d-4f3a-9d2b-27d58db4a994)

Most of the relations are minute with 2 exceptions:
  - The correlation of between Item_outlet_sales and item maximum_retail_price
  - The correlation between item_visibility and item_outlet_sales





# Models Evaluated & Results

* Linear Regression Model (Testing Set):

  ☛ MAE = 804.120
  
  ☛ MSE = 1,194,349.715

  ☛ RMSE = 1,092.863

  ☛ R^2 = 0.567
  
* Random Forest Regressor Model (Testing Set):

  ☛ MAE = 767.014

  ☛ MSE = 1,220,320.148

  ☛ RMSE = 1,104.681

  ☛ R^2 = 0.558
  
* Tuned Random Forest Regressor Model (Testing Set):

  ☛ MAE = 738.031

  ☛ MSE = 1,129,132.909

  ☛ RMSE = 1,062.607

  ☛ R^2 = 0.591

  
* The Final Model Chosen was a Random Forest Regressor Model with a max_depth of 10 and tunned n_estimators as 100

* For the testing set on the model, 59.1% of the variance in y was explained by x.

* The Mean Absolute Error was off by about 738.031

* The Mean Squared Error was 1,129,132.909

* The Root Mean Squared Error had a calculation of 1,062.607

Using this model to make predictions about the best places to live and which careers to choose to earn the most money would not be a very reliable. Considering the previous regression metrics from how the model performed, there is a disparity between the R^2 score and also the Root Mean Squared Error that cannot be ignored.


# Recommendations

Sales Prediction Insights

  * Retailers should try as much as possible to maintain accuracy while collecting data. Incomplete data could result in elimination leading to a loss of insight and deficient  deductions on the variances within the data itself
  * Also the features collected should be significant to the sought after goal. Irrelevant features with weak correlations just end up damaging the models and affect the predictions
  * Finally retailers should not only be actively engaged in observing market place trends but also be able to shift accordingly when required.

Model Performance

* Overall, the best model is definitely the tuned Random Forest Regressor Model. The model performs better than the linear regression model despite the existent bias within it.
