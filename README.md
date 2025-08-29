# 🏏 IPL Exploratory Data Analysis (EDA)

This project presents a comprehensive **Exploratory Data Analysis (EDA)** of the Indian Premier League (IPL), uncovering trends, player stats, match insights, and team performances across all IPL seasons.

---

## 🎯 Project Goals

The primary objectives of this project are to explore and visualize IPL data in order to answer key questions:

* Which team has scored the most 200+ totals?
* Which team has the highest winning percentage?
* Who has won the most "Player of the Match" (MOM) awards?
* Is there a lucky venue for a particular team?

---

## 📊 Data Sources

The analysis uses **two datasets**, which were merged using the `id` column to form a unified DataFrame:

* [Deliveries Dataset](https://drive.google.com/file/d/1O6E5DBDSFYSK4D9kandO-ELgFV23GVyi/view?usp=sharing)
* [Match Dataset](https://drive.google.com/file/d/1tfdKTH39s8bhpRbY_Sz5FYO6IRPoFoeG/view?usp=sharing)

---

## 🧾 Dataset Details

### 1. **Match Dataset (`match_dataset.csv`)**

High-level match information:

| Column               | Description                                 |
| -------------------- | ------------------------------------------- |
| `id`                 | Unique match ID (Primary Key)               |
| `city`               | Match location                              |
| `date`               | Date of the match                           |
| `player_of_match`    | Player awarded "Man of the Match"           |
| `venue`              | Stadium name                                |
| `neutral_venue`      | Whether venue was neutral (0 = No, 1 = Yes) |
| `team1`, `team2`     | Competing teams                             |
| `toss_winner`        | Team that won the toss                      |
| `toss_decision`      | Toss decision (bat/field)                   |
| `winner`             | Match-winning team                          |
| `result`             | Type of result (runs, wickets, tie)         |
| `result_margin`      | Margin of victory                           |
| `eliminator`         | Whether match was an eliminator (Y/N)       |
| `method`             | If DLS method was applied                   |
| `umpire1`, `umpire2` | Names of umpires                            |

---

### 2. **Deliveries Dataset (`deliveries_dataset.csv`)**

Ball-by-ball data:

| Column                                     | Description                         |
| ------------------------------------------ | ----------------------------------- |
| `id`                                       | Match ID (Foreign Key)              |
| `inning`                                   | Inning number (1/2)                 |
| `over`, `ball`                             | Over and ball number                |
| `batsman`, `non_striker`                   | Players involved in batting         |
| `bowler`                                   | Bowler name                         |
| `batsman_runs`, `extra_runs`, `total_runs` | Runs scored                         |
| `non_boundary`                             | Indicates non-boundary runs (0/1)   |
| `is_wicket`                                | Wicket taken (0/1)                  |
| `dismissal_kind`                           | Type of dismissal                   |
| `player_dismissed`                         | Batsman dismissed                   |
| `fielder`                                  | Fielder involved                    |
| `extras_type`                              | Type of extra (e.g., wide, no-ball) |
| `batting_team`, `bowling_team`             | Teams involved                      |

---

## 🛠️ Tools & Technologies Used

* **Jupyter Notebook / Google Colab** – For interactive analysis
* **Pandas** – Data manipulation and cleaning
* **Matplotlib & Seaborn** – Data visualization

---

## 💡 Key Insights

Here are some significant findings from the EDA:

* **Top Batsmen**: Identified top 10 run-scorers in IPL history.
* **Top Bowlers**: Showcased leading wicket-takers and their statistics.
* **Winning Teams**: Highlighted teams with the highest number of wins and best win percentages.
* **Toss Influence**: Notable correlation between toss outcomes and match results.
* **Venue Analysis**: Determined which stadiums are high-scoring or have been lucky for specific teams.

---

## ▶️ How to Run This Project

To explore this analysis on your local system or Google Colab:

1. Clone or download the repository.
2. Ensure required libraries are installed:
   `pandas`, `matplotlib`, `seaborn`
3. Open **`Assignment2Python.ipynb`** in Jupyter Notebook or Google Colab.
4. Run the notebook cells sequentially to view the analysis and visualizations.

---
