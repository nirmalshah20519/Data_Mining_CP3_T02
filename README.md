# Task 2: Predicting Finalist Teams and Players

## Task 2(A): Finalist Teams Prediction

### Feature to Predict: "Finalist" in `points_table`

The "Finalist" column in the `points_table` is the feature we aim to predict. It contains the names of the teams that will be present in the final match of the ICC Cricket World Cup 2023. The prediction will be based on the top two teams in the `points_table`, indicating the teams playing in the final.

## Task 2(B): Player Selection Prediction

### Features to Create and Predict: "Selected" in Combined DataFrame

1. **Combining DataFrames**: We merge the "deliveries" and "matches" dataframes to create a combined dataframe, bringing together detailed information about deliveries and overall match data.

2. **New Features Creation**: We introduce a new feature named "Selected" in the combined dataframe. This feature represents the players who are likely to be selected for the final match.

3. **Removing Unnecessary Features**: To streamline the dataset and focus on relevant information, we remove unnecessary features from the combined dataframe. This ensures that the model is trained on the most critical factors influencing player selection.

4. **Handling Null Values**: Null values within the dataset are filled using the mean of the particular feature. This step is crucial to ensure the completeness of the data for accurate predictions.

### Code Snippets:

#### Merging DataFrames:

```python
# Assuming df_deliveries and df_matches are the deliveries and matches dataframes
combined_df = pd.merge(df_deliveries, df_matches, on='common_column', how='inner')
