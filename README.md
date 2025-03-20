# NCAA_prediction_Machinelearningmodel_2025
NCAA Tournament Prediction - Kaggle Hackathon 2025
This repository contains the solution for the Kaggle March Machine Learning Mania 2025 competition. The objective is to predict the outcomes of NCAA basketball tournament games by applying machine learning models with advanced feature engineering and ensemble boosting techniques.

Model Overview
Algorithm: Stacked ensemble model with the following base learners:
RandomForest
GradientBoosting
AdaBoost
XGBoost
LightGBM
Meta-model: LightGBM classifier for improved accuracy.
Metrics Used:
Log Loss: Measures the accuracy of probabilistic predictions.
Brier Score: Evaluates the accuracy of predicted probabilities.
Feature Engineering
Merged regular season and tournament results for comprehensive training data.
Created advanced features:
Average, max, min, and standard deviation of winning and losing scores.
Total overtime wins.
Seeding information for each team.
Handled missing values and ensured proper data formatting.
Dataset
The data is fetched directly from Kaggle using the Kaggle API.
Datasets used:
MTeams.csv: Team information.
MSeasons.csv: Season details.
MRegularSeasonCompactResults.csv: Regular season game results.
MNCAATourneyCompactResults.csv: Tournament results.
MNCAATourneySeeds.csv: Team seed rankings.
SampleSubmissionStage2.csv: Kaggle submission format.
How to Run
Install required libraries by running:
nginx
Copy
Edit
pip install -r requirements.txt
Execute the script:
css
Copy
Edit
python main.py
The model generates predictions and saves them in a CSV file:
Copy
Edit
submission7.csv
Evaluation
The model is trained on both regular season and tournament data, providing a comprehensive view of team performance.
It uses stratified cross-validation to ensure balanced class representation.
The final predictions are formatted according to the Kaggle submission format.
Usage
The output file submission7.csv is ready for direct submission to the Kaggle competition.
The model is optimized for accuracy and efficiency, balancing performance with runtime.






