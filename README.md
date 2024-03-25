## Creative Gaming: Propensity-to-Buy Modeling

We run the advanced analytics team for Creative Gaming. We have been tasked to use telemetry data to increase awareness of the Zalon campaign. To get started, we have assembled a dataset of 30,000 Space Pirates gamers (i.e., users) named “data/cg_organic.rds”. Each row of data contains information for a single current gamer.

- Target/Outcome Variable

For each Space Pirates gamer, the data contains a variable that recorded whether the gamer had purchased the Zalon campaign since its release two months ago. The variable is named “converted.”

- Features/Explanatory Variables

The data also contains 19 features that describe the behavior and gameplay of each Space Pirates gamer since Space Pirates’ release.

- Task

Mi Haruki has asked us to build a model that uses the Space Pirates data (described in the main case) to predict which Space Pirates gamers are more (less) likely to purchase the Zalon campaign.

- Part I: Exploratory Analytics (2 points)

To gain an understanding of whether the data is appropriate for predictive analytics, engage in some exploratory analytics.

- Part II: Predictive Model (5 points)

Train a logistic regression model using all features and use the “training” variable to set a filter (“training == 1”).

- Part III: The Ad-Experiment (12 points)

We have finished building a logistic regression model to predict what kind of Space Pirates gamers were more or less likely to purchase the Zalon campaign. After debriefing Mi Haruki on the performance of the predictive model, she lays out the next steps:

“We will test the effectiveness of the in-app ad and the predictive model by exposing a random 150,000 customers to a 2-week ad campaign and measuring their conversion to Zalon over the next 2 months. At the same time, we will randomly pick another 30,000 customers and observe their organic upgrade behavior over the same period. This set of customers will not be served any in-app ads.

I want you to compare three groups based on this data.

  - Group 1: The randomly picked 30,000 Space Pirates gamers who did not receive in-app ads during the experimental period.
  
  - Group 2: A randomly picked 30,000 Space Pirates gamers among the 150,000 who were served in-app ads for Zalon.
  
  - Group 3: A model-selected 30,000 Space Pirates gamers among the 120,000 (after taking out Group 2) who were served in-app ads for Zalon.

Please report back to me how well the ads are working in terms of conversion rates and profits and by how much the model improves these metrics, all based on targeting 30,000 customers. To calculate profits, please use revenues of $14.99 from selling Zalon. The cost of serving ads to a consumer for 2 weeks is $1.50 in lost coin purchases.”

- Part IV: Better Data, Better Predictions

Mi Hiruki called for a meeting to discuss next steps. She explained:

“Before we roll out the campaign globally, we want to see whether we can use the experimental data to retrain the model. The idea is to model trial in response to the in-app ad—not just organic conversion as we did initially. We know that the in-app ad, on average, increases Zalon conversions. However, if the in-app ad works for people who would not have purchased the Zalon campaign organically, updating the model based on the in-app ad data should improve predictive performance.
Let’s retrain the model based on the randomly chosen Space Pirates gamers we messaged in the experiment and see how well the updated model compares to the original model in a test sample."

- Part V: Better Models, Better Predictions (6 points)

Mi Haruki was impressed by how much performance improved when model was retrained on the ad treatment data rather than organic data. However, she knew that the analytics team was not done yet:

“I know we have been trying to keep the models simple and perhaps the logistic regression is what we go with. However, I want to you apply machine learning models to see if they can help improve our predictions and performance further."
