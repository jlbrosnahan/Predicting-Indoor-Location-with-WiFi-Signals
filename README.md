# Smart Phone Location Predictions using WiFi Signal Data
Build an algorithm to predict an individual's location using their Smart Phone and WiFi signals? 

Do so with a relatively high level of accuracy, precision, and recall per Client Minimum Specifications? 

Check and check.

See "Location Predictions Analysis" above for Python Pipeline Analysis.

## Background
My client is developing a system to help people navigate a complex, unfamiliar interior space on a college campus.
They want me to investigate the feasibility of using WiFi fingerprinting to determine a person's indoor location.
If a model meets or exceeds minimum specifications, it will be incorporated into a Smart Phone app for indoor locationing on a University campus.

## Business Objectives
1. Build multiple different models to predict a person’s location in indoor college campus spaces using Wifi signal data
2. Answer the business question, “Can a model be built that predicts indoor location on a college campus that meets the Client’s minimum specifications?” 
3. If a model can be built meeting minimum specifications, deploy algorithm into smart phone indoor locationing app.

## Skills
* Python/Jupyter Notebook IDE
* Multiple machine learning algorithms: Support Vector Machines, Decision Trees, Random Forest, K Nearest Neighbors
* Understanding the business problem and answering the business questions (classification vs. regression)
* Feature Engineering
* Sampling techniques and feature selection strategies for large dataset
* Dimensionality reduction/ zero variance variable removal
* Cross validation, parameter tuning, and post-resample comparison of model metrics for highly multi-class classification problem
* Using metrics and recall investigation for determining optimal algorithm(s) for model deployment
* Business objectives solved

## Client Minimum Specifications
* Indoor location must be as precise as predicting within 10-15 feet of the indoor room, also defined as ‘SpaceID’ within source data. Relative position, or whether individual is outside or inside of room, is unnecessary.
* Performance metrics ideal for deployment:
  * Accuracy scores on test data reaches 80% or higher
  * Precision (accuracy of minority class) on test data reaches 80% or higher
  * Recall (coverage of minority class) on test data is 80% or higher
  * F1 Score for multi-class problem achieves 80% or higher

## Data Description
Data was collected by 20 individuals using mobile phone devices on a college campus in Velencia, Spain. The data source is the UJIIndoorLoc WLAN database
* 19937 observations of  529 variables
* 520 of the variables (98% of dataset) are homogenous wifi-access points providing numeric values representing signal strength
* 9 remaining variables are Longitude, Latitude, Floor, BuildingID, SpaceID, Relative Position, UserID, PhoneID, and Time
* Contains no missing values

## Insights and Model Recommendation
* Random Forest algorithms overall met or exceeded client minimum specification metrics for predicting WiFi locations on a college campus. 
* Recall for location predictions on individual building datasets was higher than OOB dataset.
* Recommend deploying Random Forest algorithms by individual buildings for Indoor Locationing smart phone app

## Post-resample Performance Comparison of All Models
![Visual 1](https://github.com/jlbrosnahan/Predict-Sales_Volume/blob/master/Rplot02.jpeg)

## Absolute Recall Performance Comparison of Random Forest Models


