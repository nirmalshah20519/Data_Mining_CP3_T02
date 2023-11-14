# IDM Project-3 - Team-02

# Data Mining Project: ICC Cricket World Cup 2023 Prediction


### Team Members:
- Nirmal Shah 202311043
- Samarth Motka 202311023
- Darshit Kalariya 202311035
- Deepak Khatri 202311042
- Viraj Prajapati 202311069

## Task 1: Predicting Number of No Balls and Total Runs Scored in Final Match

### Task Overview:


1. **Predicting Number of No Balls:**
   - Handling null values by replacing them with 0.
   - Exploring unique values in each column.
   - Selecting 'noballs' as the target variable.
   - Applying one-hot label encoding.
   - Standardizing the data.
   - Training a linear regression model.
   - MSE: 1.9230769230769367.
   - Testing the model on the final match data obtained in Task 3, predicting 1 no ball.

2. **Predicting Total Runs Scored:**
   - Handling null values by replacing them with 0.
   - Creating columns for total runs, runs off bat, extras, wides, no balls, byes, leg-byes, etc.
   - Merging the columns with the data frame.
   - Applying one-hot label encoding.
   - Training an XGBoost model.
   - MSE: 3541.0766141535355.
   - Testing the model on the final match data obtained in Task 3, predicting Team India will score 304 runs in the 1st innings.

### GitHub README:

#### Task 1(A): Predicting Number of No Balls
- Handle null values by replacing them with 0.
- Explore unique values in each column.
- Select 'noballs' as the target variable.
- Apply one-hot label encoding.
- Standardize the data.
- Train a linear regression model.
  - Mean Squared Error: 1.92
- Test the model on the final match data, predicting 1 no ball.

#### Task 1(A): Predicting Total Runs Scored
- Handle null values by replacing them with 0.
- Create columns for total runs, runs off bat, extras, wides, no balls, byes, leg-byes, etc.
- Merge the columns with the data frame.
- Apply one-hot label encoding.
- Train an XGBoost model.
  - Mean Squared Error: 3541.08
- Test the model on the final match data, predicting Team India will score 304 runs in the 1st innings.


# Task 2: Predicting the Finalist Teams and Players

## Task 2(A): Predicting Finalist Teams

### Overview:
This task involves predicting the two finalist teams in the ICC Cricket World Cup 2023 and the 11 players likely to be part of each finalist team.

### Steps Taken:

1. **Data Preprocessing:**
   - Renamed the "match_number" column to "match_id" for merging.
   - Checked for null values in the "points_table" dataset.
   - Described numerical and categorical features.

2. **Encoding Categorical Features:**
   - Utilized one-hot encoding for categorical features.

3. **Prediction Model:**
   - Target variable: "Finalist" column in "points_table."
   - Model Accuracy: 50%.

## Task 2(B): Predicting Finalist Players

### Overview:
This subtask involves predicting the 11 players for each finalist team by combining the "deliveries" and "matches" dataframes.

### Steps Taken:

1. **Combined Dataframe:**
   - Merged "deliveries" and "matches" based on a common column.
   - Created a new feature named "Selected" for predicting selected players.

2. **Data Preprocessing:**
   - Removed unnecessary features.
   - Filled null values with the mean of the respective feature.

3. **Prediction Model:**
   - Target variable: "Selected" column.
   - Model Accuracy: 85.70%.



## Overview:

This machine learning project focuses on predicting the finalists and winners of the ICC Cricket World Cup 2023. The project is divided into Exploratory Data Analysis (EDA) and Model Building phases.

## Exploratory Data Analysis (EDA):

### Data Preparation:

1. **Reading and Storing CSV Files:**
   - All CSV files related to the World Cup are read and stored for analysis.

2. **Analysis of Matches in India:**
   - The dataset is filtered to include only matches in India, providing insights specific to the host country.

### Data Visualization:

3. **Top 5 Run Scorers at Different Venues:**
   - Visualizes the top 5 run-scorers at various cricket venues.

4. **Top 5 Wicket Takers at Different Venues:**
   - Analyzes and visualizes the top 5 wicket-takers at different cricket venues.

5. **Wins by Teams at Different Venues:**
   - Stacked bar chart showcasing the number of wins by cricket teams at different venues.

6. **Chase vs. Defend Analysis:**
   - Grouped bar chart comparing the frequency of match results (chase vs. defend) at various venues.

7. **Team-wise Win Percentage:**
   - Pie chart displaying the percentage of wins for each team.

8. **Toss Impact Analysis:**
   - Bar plot exploring the relationship between winning the toss and winning the match.

9. **Toss Decision Impact:**
   - Count plot showcasing the number of matches won based on the toss decision.

10. **Batting and Bowling Performance:**
    - Dual analysis of batting and bowling performances, displaying batting and bowling averages for each team.

## Model Building:

### 1. Logistic Regression Model:
   - Train Accuracy: 81.2%
   - Test Accuracy: 62.5%

### 2. Support Vector Classifier:
   - SVM Train Accuracy: 81.2%
   - SVM Test Accuracy: 62.5%

### 3. Random Forest Model:
   - Random Forest Train Accuracy: 100%
   - Random Forest Test Accuracy: 75%

### Dataset Preparation:

11. **Historical Match Dataset Enhancement:**
    - Prepares the historical match dataset by adding win scores for participating teams based on city-specific performance data.

12. **Winning Team Encoding:**
    - Creates a new column ('winning_team') indicating the winning team as '0' (Team 1) or '1' (Team 2). The dataset is split into training and testing sets.

### Neural Network Model:

13. **Neural Network Architecture:**
    - Implements a simple neural network for binary classification to predict the winning team in cricket matches based on historical features.

## Prediction of Semi-Finals:

14. **India vs New Zealand:**
    - Predicts the winner and winning chances for the semi-final clash in Mumbai.

15. **South Africa vs Australia:**
    - Predicts the winner and winning chances for the semi-final matchup in Kolkata.

16. **Predicted Finalists:**
    - After analyzing semi-final predictions, anticipates the finalists for the championship clash.

## Prediction of Finals:

17. **India vs Australia:**
    - Predicts the winner and winning chances for the final match in Ahmedabad.

18. **Final Predictions:**
    - Summarizes the predicted finalists and the anticipated winner of the championship title.

## Conclusion:

This machine learning project combines data analysis and predictive modeling to provide insights into the ICC Cricket World Cup 2023. The EDA phase explores various aspects of matches in India, while the model-building phase utilizes a neural network for predicting match outcomes.

Feel free to customize the content based on specific details or requirements for your project.
