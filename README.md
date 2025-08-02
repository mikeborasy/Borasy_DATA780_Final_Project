# Borasy_DATA780_Final_Project
Predicting MLB game outcomes using supervised machine learning on 2025 team-level statistics. Final project for DATA 780 at UNC Chapel Hill, featuring feature engineering, random forest classification, and real-world evaluation on July matchups.

# MLB Game Outcome Prediction — DATA 780 Final Project

This project applies supervised machine learning techniques to predict the outcome of MLB games using 2025 team-level statistics. It was completed as a final individual project for the graduate-level course DATA 780 at UNC Chapel Hill MADS Masters Program. 

## Description

The goal of this project is to forecast whether the home team will win a given MLB matchup based on statistical differences between the home and away teams. Features were engineered from offensive (OPS), defensive (ERA), and WAR-related metrics. The final model was evaluated on real 2025 games played between July 18 and July 28.

## Files Included

- `Borasy_DATA_780_Final_Project.ipynb` — Jupyter Notebook with all code, modeling, feature engineering, and evaluation
- `MLB_Prediction_Final_Report.pdf` — NeurIPS-style summary report of methods, results, and conclusions
- `mlb_2025.csv` — Cleaned 2025 team stats used for prediction
- `README.md` — Project overview and submission details

## Summary

We trained and compared three classification models:
- Random Forest (best performer): 65% accuracy
- Logistic Regression: ~55% accuracy
- Gradient Boosting: ~50% accuracy

The final model used engineered features such as OPS difference, WAR difference, and binary indicators like `Better_OPS` and `Better_WAR`. Accuracy was validated on 74 manually entered July 2025 matchups.

## Features Used

- `OPS_Diff`, `ERA_Diff`, `WAR_Diff`, `RunDiff_Diff`, `WHIP_Diff`, `Fld_Diff`
- Binary indicators: `Better_OPS`, `Better_WAR`, `Better_ERA`

## Data Sources

All team statistics were scraped from Baseball Reference:

- [2025 Standard Batting](https://www.baseball-reference.com/leagues/MLB/2025-standard-batting.shtml)
- [2025 Standard Pitching](https://www.baseball-reference.com/leagues/MLB/2025-standard-pitching.shtml)
- [2025 Wins Above Average by Position](https://www.baseball-reference.com/leagues/MLB/2025-winsaboveaverage.shtml)
- [2025 Fielding](https://www.baseball-reference.com/leagues/MLB/2025-standard-fielding.shtml)

Game results for July 18–28, 2025 were manually recorded and used to evaluate model accuracy.

## Author

Michael Borasy  
Graduate Data Science Program  
University of North Carolina at Chapel Hill

