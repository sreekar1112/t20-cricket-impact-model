# Context-Aware Performance Analytics Framework for The Hundred (Women’s Cricket)

This project develops a **context-aware cricket analytics framework** to evaluate player performance beyond traditional metrics such as batting average, strike rate, and wickets taken.

Traditional statistics summarize outcomes but often ignore **match context, pressure situations, and the timing of contributions**. In short-format cricket, these contextual factors strongly influence match outcomes.

This project introduces a **ball-by-ball analytical approach** to quantify the real impact of batting and bowling performances.

---

# Project Objectives

- Evaluate batting and bowling performance at **match level**
- Incorporate **match pressure and phase difficulty**
- Extend match ratings to **tournament-level evaluation**
- Identify **top batters, top bowlers, and tournament MVPs**
- Provide **transparent and explainable cricket analytics**

---

# Key Metrics

## Batting Impact Metrics

Batting impact is evaluated using context-aware features such as:

- **Phase Weighted Runs** – weighting runs based on match phase
- **Boundary Impact Score (BIS)** – momentum impact of boundaries
- **Dot Ball Cost (DBC)** – pressure created by dot balls
- **Unified Pressure Index (UPI)** – difficulty of match situation

Final batting rating:
BattingRating = (PDB + 8 × BIS − 6 × DBC − DP) × UPI


---

## Bowling Impact Metrics

Bowling performance is evaluated using:

- **Wicket Impact Score (WIS)** – value of wickets depending on phase
- **Run Pressure Index (RPI)** – control over scoring rate
- **Dot Ball Pressure (DBP)**
- **Bowling Control Index (BCI)**

Final bowling rating:
BowlingRating = (20 × WIS + 15 × RPI + 10 × DBP + 10 × BCI + 5 × DODB) × UPI

---

# Tournament-Level Evaluation

Match ratings are aggregated across matches to evaluate **consistent performers**.

Tournament impact score:AvgRating × Consistency × Experience

Where:

- **Consistency** = 1 − (StdRating / AvgRating)  
- **Experience** = log(1 + MatchesPlayed)

This rewards players who perform consistently across the tournament.

---

# MVP Identification

Tournament MVP is calculated using combined batting and bowling contributions.
MVP = 0.6 × BattingRating + 0.4 × BowlingRating

This balances batting and bowling impact to identify the **most valuable player of the tournament**.

---

# Repository Structure

t20-cricket-impact-model
│
├── notebooks
│ ├── batting_impact_model.ipynb
│ ├── bowling_impact_model.ipynb
│ └── tournament_impact_analysis.ipynb
│
├── presentation
│ └── hundred_cricket_impact_analysis_report.pdf
│
├── data
│ └── dataset_information.md
│
├── results
│
└── README.md


---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

# Data Sources

The analysis uses **ball-by-ball cricket datasets** derived from publicly available sources such as:

- Cricsheet
- ESPN Cricinfo match scorecards

These datasets allow precise evaluation of **match context and player impact**.

---

# Example Outputs

The project generates:

- Match-level batting impact leaderboards
- Match-level bowling impact rankings
- Tournament-level player rankings
- MVP evaluation visualizations

---

# Key Contribution

This project demonstrates that **cricket performance can be evaluated more accurately using context-aware metrics rather than simple aggregates**.

By combining ball-by-ball analytics with tournament-level evaluation, the framework provides a **transparent and explainable approach to identifying match-winning performances**.

---

# Author

**Sreekar Regulavalasa**

Sports Data Analyst | Cricket Analytics  
Computer Science Engineering – GITAM University

