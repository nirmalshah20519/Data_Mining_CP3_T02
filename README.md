# Data Mining Project: ICC Cricket World Cup 2023 Prediction

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
