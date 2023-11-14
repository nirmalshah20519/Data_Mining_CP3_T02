# IDM Project-3 - Team-02

## Task 1: Predicting Number of No Balls and Total Runs Scored in Final Match

### Team Members:
- Nirmal Shah 202311043
- Samarth Motka 202311023
- Darshit Kalariya 202311035
- Deepak Khatri 202311042
- Viraj Prajapati 202311069

### Task Overview:
1. **Predicting Number of No Balls:**
   - Handling null values by replacing them with 0.
   - Exploring unique values in each column.
   - Selecting 'noballs' as the target variable.
   - Applying one-hot label encoding.
   - Standardizing the data.
   - Training a linear regression model.
   - MSE: 1.9230769230769367.
   - Testing the model on the final match data, predicting 1 no ball.

2. **Predicting Total Runs Scored:**
   - Handling null values by replacing them with 0.
   - Creating columns for total runs, runs off bat, extras, wides, no balls, byes, leg-byes, etc.
   - Merging the columns with the data frame.
   - Applying one-hot label encoding.
   - Training an XGBoost model.
   - MSE: 3541.0766141535355.
   - Testing the model on the final match data, predicting Team India will score 304 runs in the 1st innings.
