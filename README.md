# README

## QRT Data Challenge: Match Result Prediction

### Overview

This is a solution to QRT's Data Challenge 2024. This project focuses on predicting the outcome of football matches using real historical data at the player, team, and league levels. The challenge requires building predictive models capable of determining the winner or if the match will result in a draw, across various leagues worldwide.

### Table of Contents
- [Project Structure](#project-structure)
- [Data Description](#data-description)
- [Modeling Approach](#modeling-approach)
- [Evaluation](#evaluation)
- [Collaboration](#collaboration)

### Project Structure
### Data Description

Data at the team and player levels for numerous football leagues is provided for this challenge. Due to the size of the dataset, it is excluded from this repository and must be downloaded from the following link: [Challenge Data](https://challengedata.ens.fr/participants/challenges/143/).

The data is divided into two zip files, `X_train.zip` and `X_test.zip`, and two CSV files, `Y_train.csv` and `Y_train_supp.csv`.

#### Team Data

**Identifiers:**
- `ID`
- `LEAGUE` (not included in test data)
- `TEAM_NAME` (not included in test data)

**Statistics (aggregated by sum, average, and standard deviation):**
- `TEAM_ATTACKS`
- `TEAM_BALL_POSSESSION`
- `TEAM_BALL_SAFE`
- `TEAM_CORNERS`
- `TEAM_DANGEROUS_ATTACKS`
- `TEAM_FOULS`
- `TEAM_GAME_DRAW`
- `TEAM_GOALS`
- `TEAM_YELLOWCARDS`
and more...

#### Player Data

**Identifiers:**
- `ID`
- `LEAGUE` (not included in test data)
- `TEAM_NAME` (not included in test data)
- `POSITION`
- `PLAYER_NAME` (not included in test data)

**Statistics (aggregated by sum, average, and standard deviation):**
- Similar to team statistics but more detailed.

### Modeling Approach

#### Data Preprocessing

1. **Data Cleaning:**
   - Handle missing values.
   - Remove irrelevant columns.

2. **Data Integration:**
   - Merge data from different sources if necessary.
   - Ensure data consistency.

3. **Normalization/Standardization:**
   - Scale numerical features as needed.

#### Feature Engineering

1. **Feature Selection:**
   - Identify relevant features for prediction.

2. **Feature Transformation:**
   - Encode categorical variables.
   - Create new features from existing ones if beneficial.

#### Models

1. **Model Selection:**
   - Choose appropriate models for prediction (e.g., Logistic Regression, Random Forest, Neural Networks).
### Evaluation
### Collaboration

