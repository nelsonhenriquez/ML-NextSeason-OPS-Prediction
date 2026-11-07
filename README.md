# ML-NextSeason-OPS-Prediction

## Overview
A machine learning project predicting Major League Baseball (MLB) player performance (OPS) for the next season using historical datasets.

<img width="701" height="550" alt="image" src="https://github.com/user-attachments/assets/b3224008-1772-40a0-abab-3a499d9a09bd" />

## Features
- Data cleaning, preprocessing, and feature engineering (OBP, SLG, OPS, and age)
- Exploratory data analysis with Pandas and Seaborn
- Predictive models including Linear Regression and Random Forest
- Chronological train/test split to avoid training on future seasons
- Model evaluation with R², MAE, and RMSE metrics
- Visualizations to identify trends and key predictors

## Data
Historical batting, pitching, and player records from the Lahman Baseball Database (`Batting.csv`, `People.csv`, and `Pitching.csv`). The final dataset covers hitters with at least 250 plate appearances in a season, with pitchers removed, for 15,259 player seasons from 1954 to 2024.

## Technologies Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook

## Results
Models were trained on seasons before 2005 (10,976 samples) and tested on 2005 and later (4,283 samples). Linear Regression slightly edged out Random Forest on the test set.

| Model | R² | MAE | RMSE |
|---|---|---|---|
| Linear Regression | 0.217 | 0.087 | 0.126 |
| Random Forest | 0.213 | 0.088 | 0.126 |

## How to Run
1. Clone the repo  
2. Install dependencies with `pip install -r requirements.txt`  
3. Open `ml_final.ipynb` in Jupyter Notebook or JupyterLab  
4. Run each cell sequentially to train, evaluate, and visualize the models  

## Visualizations
The notebook includes feature histograms, an OPS distribution plot, a correlation heatmap, predicted vs actual plots for both models, and Random Forest feature importance.

## Topics / Tags
`machine-learning` `python` `mlb` `predictive-analytics` `data-analysis`
