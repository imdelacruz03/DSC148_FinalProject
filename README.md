# Predicting NCAA Women's March Madness Tournament Outcomes Using Machine Learning

**DSC 148 — Intro to Data Mining | UCSD | June 2026**  
**Author:** Isabela de la Cruz

## Overview
This project applies machine learning to predict game outcomes in the NCAA 
Women's Basketball Tournament using a binary game-level matchup framework.

## Research Question
Can regular season and conference tournament statistics predict NCAA Women's 
March Madness tournament outcomes, and what team characteristics best separate 
winners from losers?

## Key Results
- **Best Model:** XGBoost — 80.22% per-game accuracy
- **Perfect Bracket Probability:** 1 in 1,068,732 (vs. 1 in 9.2 quintillion random)
- **2025 Champion (UConn):** Correctly ranked #1 in Monte Carlo simulations (16.6%)
- **2026 Champion (UCLA):** Correctly ranked #2 in Monte Carlo simulations (19.6%)
- **Key Finding:** Seed number and scoring margin are the strongest predictors;
  3PT% is a weak predictor contrary to initial hypothesis

## Dataset
- Source: Kaggle March Machine Learning Mania 2026
- Training: 151,130 game matchups (regular season + conference + NCAA tournament)
- Test: 268 NCAA tournament games (2024-2026)

## Models
| Model | Accuracy | F1 Score |
|---|---|---|
| Logistic Regression (Baseline) | 65.30% | 65.30% |
| Random Forest | 79.85% | 79.85% |
| XGBoost | **80.22%** | **80.22%** |

## Files
- `ncaa_womens_march_madness.ipynb` — Main analysis notebook
- `fig1_feature_correlation.png` — Feature correlation analysis
- `fig2_3pt_by_round.png` — 3PT% by tournament round
- `fig3_model_comparison.png` — Model performance comparison
- `fig4_monte_carlo.png` — Monte Carlo bracket simulations
- `fig5_feature_importance.png` — Random Forest feature importances

## Requirements
```
pandas
numpy
scikit-learn
xgboost
matplotlib
seaborn
```
