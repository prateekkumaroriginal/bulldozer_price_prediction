# bulldozer_price_prediction

# Predicting the sales price of bulldozers using Machine Learning.
## 1. Problem Definition:
How well can we predict the sales price of a bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?
## 2. Data:
The data is downloaded from the Kaggle Bluebook for Bulldozers competition: https://www.kaggle.com/c/bluebook-for-bulldozers/data

There are 3 main datasets:

* **Train.csv** is the training set, which contains data through the end of 2011.
* **Valid.csv** is the validation set, which contains data from January 1, 2012 - April 30, 2012 You make predictions on this set throughout the majority of the competition. Your score on this set is used to create the public leaderboard.
* **Test.csv** is the test set, which won't be released until the last week of the competition. It contains data from May 1, 2012 - November 2012. Your score on the test set determines your final rank for the competition.

## 3. Evaluation:
The evaluation metric for this competition is the RMSLE (root mean squared log error) between the actual and predicted auction prices.

For more on the evaluation of this project check: https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation

Note: The goal for most regression evaluation metrics is to minimize the error. For example, our goal for this project will be to build a machine learning model which minimises RMSLE.

## 4. Features:
Kaggle provides a data dictionary detailing all of the features of the dataset. You can view this data dictionary on Google Sheets: https://docs.google.com/spreadsheets/d/18ly-bLR8sbDJLITkWG7ozKm8l3RyieQ2Fpgix-beSYI/edit?usp=sharing

## Final model parameters
- n_estimators=40,
- min_samples_leaf=1,
- min_samples_split=14,
- max_features=0.5,
- max_samples=None

## Final model scores:
- `Training MAE`: 2953.8161137163484,
- `Validation MAE`: 5951.247761444453,
- `Training RMSLE`: 0.14469006962371858,
- `Validation RMSLE`: 0.24524163989538328,
- `Training r2`: 0.9588145522577225,
- `Validation r2`: 0.8818019502450094

## Feature Importances:
![image](https://github.com/prateekkumaroriginal/bulldozer_price_prediction/assets/89418989/91a8617b-e8f0-4512-a965-a4debdb59d11)
