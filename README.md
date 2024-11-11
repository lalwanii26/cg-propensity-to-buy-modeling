# Creative Gaming: Propensity-to-Buy Modeling for the Zalon Campaign

## Overview
In collaboration with Creative Gaming, I have leveraged telemetry data from "Space Pirates" to enhance the Zalon campaign's visibility. Utilizing a dataset of 30,000 gamers, we embarked on creating predictive models to pinpoint which players are more likely to engage with the Zalon campaign.

### Dataset
- **File Name**: `data/cg_organic.rds`
- **Size**: 30,000 rows (each row represents a gamer)
- **Features**: 19 gameplay and behavior features per gamer
- **Target Variable**: `converted` (indicates whether a gamer has purchased the Zalon campaign)

## Task Breakdown

### Part I: Exploratory Analytics
Evaluate the suitability of the dataset for predictive analytics.

### Part II: Predictive Model
Develop a logistic regression model using the dataset, filtered by `training == 1`, to predict the likelihood of purchasing the Zalon campaign.

### Part III: The Ad-Experiment
Conduct a controlled experiment to test the effectiveness of in-app ads:
- **Group 1**: 30,000 gamers without ad exposure (control group)
- **Group 2**: 30,000 randomly selected gamers from 150,000 who received ads
- **Group 3**: 30,000 model-selected gamers from the remaining 120,000 who received ads

**Objective**: Analyze the conversion rates and profit generated from each group. Calculate profit using a revenue of $14.99 per Zalon sale and a cost of $1.50 per gamer for ad exposure.

### Part IV: Better Data, Better Predictions
Retrain the logistic regression model with data from the ad experiment to improve its predictive accuracy.

### Part V: Better Models, Better Predictions
Explore advanced machine learning models to enhance prediction performance further.
