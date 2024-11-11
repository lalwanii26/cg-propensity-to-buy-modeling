# Creative Gaming: Propensity-to-Buy Modeling for the Zalon Campaign

## Overview
In collaboration with Creative Gaming, I leveraged telemetry data from "Space Pirates" to enhance the Zalon campaign's visibility. Utilizing a dataset of 30,000 gamers, we embarked on creating predictive models to pinpoint which players are more likely to engage with the Zalon campaign.

### Dataset
- **File Name**: `data/cg_organic.rds`
- **Size**: 30,000 rows (each row represents a gamer)
- **Features**: 19 features detailing gameplay and gamer behavior
- **Target Variable**: `converted` (indicates whether a gamer has purchased the Zalon campaign)

## Modeling Approach
### Part I: Exploratory Analytics
Initial data analysis aimed to assess the dataset’s appropriateness for predictive modeling.

### Part II: Predictive Model
A logistic regression model was developed to predict purchase likelihood, based on gameplay data filtered for training purposes.

### Part III: Ad Experiment
Conduct a controlled experiment to test the effectiveness of in-app ads:
- **Group 1**: 30,000 gamers without ad exposure (control group)
- **Group 2**: 30,000 randomly selected gamers from 150,000 who received ads
- **Group 3**: 30,000 model-selected gamers from the remaining 120,000 who received ads

**Objective**: Analyze the conversion rates and profit generated from each group. Calculate profit using a revenue of $14.99 per Zalon sale and a cost of $1.50 per gamer for ad exposure.

### Part IV: Model Retraining
Using ad-experiment data, the logistic regression model was retrained to improve its accuracy, focusing on ad-triggered purchases rather than organic behavior.

### Part V: Advanced Machine Learning Models
Further exploration was done using advanced machine learning techniques to enhance predictive accuracy:
- **Random Forest**: Employed for its robustness against overfitting, providing insights on feature importance and model stability.
- **Neural Networks**: Used to capture complex nonlinear patterns in data, significantly improving prediction accuracy over traditional models.

## Results and Conclusion
The project successfully demonstrated the application of **logistic regression**, **Random Forest**, and **Neural Network** models to predict user behavior in a gaming context. Key findings include:

- **Targeted ad exposure** based on predictive models significantly increased conversion rates and profits compared to random or no ad exposure.
- **Retraining models** with data from ad-experiments further improved predictive accuracy, showcasing the benefits of adaptive modeling in dynamic marketing campaigns.
- Advanced models like **Random Forest** and **Neural Networks** provided substantial improvements in model performance, highlighting their potential in complex scenarios involving high-dimensional data.

## Technologies Used
- Python libraries: pandas, NumPy, Matplotlib, Scikit-Learn, PyRSM
- Data analysis and predictive modeling techniques ranging from Logistic Regression, Random Forest, and Neural Networks.
