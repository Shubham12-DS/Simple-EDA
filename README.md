# IPL Exploratory Data Analysis (EDA) 🏏
This project contains an in-depth Exploratory Data Analysis (EDA) of the Indian Premier League (IPL) data. The analysis is performed to uncover interesting trends, player statistics, and match-level insights from all seasons of the tournament.

🎯 Project Goal
The primary goal of this project is to explore and visualize the IPL data to answer key questions, such as:

Which team has scored the most number of 200+ scores?

Which team has the highest winning percentage?

Who has won the most MOM awards?

Is there any lucky venue for a particular team?

📊 Data Sources
The analysis is based on two datasets containing information from the IPL matches. These two datasets were merged on a common id column to create a single, comprehensive DataFrame for analysis.

Dataset Links
Deliveries Dataset:
https://drive.google.com/file/d/1O6E5DBDSFYSK4D9kandO-ELgFV23GVyi/view?usp=sharing

Match Dataset:
https://drive.google.com/file/d/1tfdKTH39s8bhpRbY_Sz5FYO6IRPoFoeG/view?usp=sharing

Column Details
Match Dataset (match_dataset.csv)

This dataset provides a high-level view of each match, focusing on the overall outcome.

id: A unique ID for each match. This is the primary key used to link this dataset with the deliveries dataset.

city: The location where the match was played.

date: The date of the match.

player_of_match: The name of the player who won the "Player of the Match" award.

venue: The stadium where the match took place.

neutral_venue: A binary value (0 or 1) indicating if the venue was neutral.

team1 & team2: The names of the two competing teams.

toss_winner: The team that won the coin toss.

toss_decision: The decision made by the toss-winning captain (bat or field).

winner: The team that won the match.

result: The type of victory, such as runs, wickets, or tie.

result_margin: The margin of victory in terms of runs or wickets.

eliminator: A flag (Y or N) for matches that went into a super over.

method: Indicates if the Duckworth-Lewis-Stern (DLS) method was applied.

umpire1 & umpire2: The names of the two umpires for the match.

Deliveries Dataset (deliveries_dataset.csv)

This dataset provides a granular, ball-by-ball breakdown for every match, perfect for in-depth analysis of player performance.

id: The unique match ID, acting as a foreign key to link to the match dataset.

inning: The inning number (1 or 2).

over: The over number in the current inning.

ball: The ball number within the current over.

batsman: The name of the batsman on strike.

non_striker: The name of the non-striker.

bowler: The name of the bowler.

batsman_runs: The number of runs scored by the batsman on that specific ball.

extra_runs: Any additional runs from extras like wides or no-balls.

total_runs: The total runs scored on that ball.

non_boundary: A flag (0 or 1) indicating if the ball went for a boundary.

is_wicket: A flag (0 or 1) indicating if a wicket was taken.

dismissal_kind: The type of dismissal (e.g., caught, bowled).

player_dismissed: The name of the batsman who was dismissed.

fielder: The name of the fielder involved in the dismissal.

extras_type: The type of extra given.

batting_team**: The team currently batting.

bowling_team**: The team currently bowling.

🛠️ Tools & Technologies
Jupyter Notebook: The analysis is performed in a Jupyter Notebook environment (specifically, Google Colab).

Pandas: Used extensively for data loading, cleaning, and manipulation.


💡 Key Findings
The EDA process revealed several key insights into the IPL:

Batting Dominance: The analysis identified the top 10 batsmen by total runs scored in IPL history.

Bowling Prowess: It highlighted the leading wicket-takers and their key bowling metrics.

Team Success: The project showcases which teams have been the most successful in terms of wins and win percentage over the years.

Toss Impact: A clear correlation was found between winning the toss and the final match result, showing the strategic importance of the toss.

Venue Performance: The analysis pinpoints which stadiums have hosted the most matches and which venues are high-scoring.

▶️ How to Run the Notebook
To run this analysis on your local machine or in Google Colab:

Clone this repository to your local machine.

Ensure you have the required libraries installed (pandas, matplotlib, seaborn).

Open the Assignment2Python.ipynb file in a Jupyter Notebook environment.

Run the cells sequentially to see the analysis and visualizations.
