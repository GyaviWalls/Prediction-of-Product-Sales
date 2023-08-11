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

