Pipeline Stages
Stage 1: Data Ingestion
Objective
Load datasets into Pandas DataFrames.

Dataset: https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020

Tasks
Read both CSV files
Inspect:
shape
columns
data types
Expected Output
Two DataFrames:
deliveries_df
matches_df


Stage 2: Data Cleaning & Validation
Objective
Ensure data quality before analysis.

Tasks
Check for missing values
Handle or report inconsistencies
Validate:
match IDs alignment between datasets
correct data types (numeric vs categorical)
Deliverable
Cleaned DataFrames ready for processing



Stage 3: Data Transformation
Objective
Prepare data for analysis.

Tasks
Create new columns:
Total runs per ball (if extras exist, include logic)
Standardize columns:
Ensure consistent naming
Merge datasets:
deliveries_df.merge(matches_df, left_on="match_id", right_on="id")

Output
A unified DataFrame for analysis
