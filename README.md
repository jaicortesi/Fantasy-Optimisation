# Fantasy-Optimisation
Hi,

I built a Premier League fantasy football optimisation model, training XGBoost and other regression models on historical player data to predict points, then using constrained optimisation to assemble the highest-scoring squad within budget and positional limits.
The model performed well (test MSE of 0.0427), though I'd approach a few things differently now: the training data was limited to one season, I didn't account for fixture difficulty or form momentum, and the optimisation didn't consider captain selection or bench strategy. This project is exactly why I'm drawn to Stats Perform. I want to work where sports data and AI intersect at the highest level, and I'd welcome the chance to discuss how my background fits.
I've linked the notebook here: https://github.com/jaicortesi/Fantasy-Optimisation/blob/main/MATH10%20Final%20Project.ipynb

Jai Cortesi

# Fantasy Premier League Optimisation Model

A machine learning project that predicts Premier League player performance and optimises fantasy football team selection using constrained optimisation.

## Overview

Built during my Mathematics degree at UC Irvine (Fall 2024), this project:

- Trains and compares five regression models (XGBoost, Random Forest, Ridge, Lasso, Linear Regression) on historical FPL data
- Engineers features including cost-performance ratio and points-per-minute
- Uses XGBoost (best performer, test MSE: 0.0427) to predict player points
- Applies constrained optimisation to select a 15-player squad within budget and positional limits

## Key Findings

- XGBoost outperformed other models for capturing non-linear relationships in player data
- Goals scored contributed 25%+ of feature importance for attacking players
- Clean sheets and minutes dominated importance for defenders
- Cost-performance ratio emerged as a key predictor across all positions

## Tools

Python, pandas, scikit-learn, XGBoost, matplotlib, seaborn

## Data

- Training: [FPL 2023-24 Dataset](https://www.kaggle.com/datasets/meraxes10/fantasy-premier-league-dataset-2023-2024)
- Testing: [FPL 2024-25 Dataset](https://www.kaggle.com/datasets/meraxes10/fantasy-premier-league-dataset-2024-2025)
