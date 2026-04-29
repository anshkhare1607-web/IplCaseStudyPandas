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


Stage 4: Core Analysis
1. Total Runs per Match
Calculate total runs scored in each match.


2. Runs per Team per Match
Compute total runs scored by each team in every match.


3. Top 10 Batters
Identify top 10 batters based on total runs scored.


4. Strike Rate of Batters
Calculate strike rate for each batter:

Runs scored
Balls faced

5. Top 10 Bowlers by Economy
Calculate economy rate and rank bowlers.


6. Most Consistent Batters
Find batters with:

High average runs per match
Minimum number of matches played

7. Highest Individual Score in a Match
Find the highest runs scored by a batter in a single match.


8. Boundary Analysis
Total number of 4s and 6s
Top players by boundaries

9. Boundary Percentage
For each batter:

Percentage of runs coming from boundaries

10. Dot Ball Analysis
Count dot balls (runs == 0)
Identify bowlers with most dot balls

11. Runs per Over Analysis
Average runs scored in each over (1–20)
Identify high-scoring overs

12. Powerplay Performance (Overs 1–6)
Total runs in powerplay
Best teams in powerplay

13. Death Overs Performance (Overs 16–20)
Total runs
Best teams and batters in death overs
14. Run Distribution per Inning
Compare:

First inning vs second inning scoring patterns

15. Toss Impact Analysis
Compare runs scored by toss-winning team vs opponent
Analyze if toss gives advantage

16. Player of Match Contribution
Check:

Did the player of the match contribute the highest runs?

17. Venue-wise Analysis
Total matches per venue
Average runs scored at each venue
18. City-wise Scoring Trends
Average runs by city
Identify high-scoring cities

19. Season-wise Run Trends
Total runs per season
Growth or decline trends
20. Winning Team Analysis
Determine winner based on runs
Compare with actual outcomes (if available)


Stage 5: Derived Insights
Objective
Convert raw analysis into insights.

Tasks
Identify:
Most consistent batter
Best death-over team
High-scoring venues
Provide short observations (text-based)
