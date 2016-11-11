# Yelp-Reviews

10/09 Meeting with Lappas

Yelp project proposal


Topic: Changepoints and events


1. Question: Can you detect when things change suddenly (I.e a business coming under new management)? Can you see when a city starts going nuts over cronuts?


2. Data understanding:

  * Hypothesis 1: The number of reviews for a business will fluctuate dramatically given a change




3. Data preparation:
  * Json business files are loaded




4. Modeling (Per Lappas, stay away from time series):

  * For each business with at least 50 reviews:
    * Create a dict for each 1 month period and store the reviews in the dict
    * Perform a statistical test to compare the # of reviews over each dict
    * For changes that are significantly higher, isolate it, and perform a text analysis
    * Pull the phrases to see what has changed in the business




5. Evaluation:

  * Accuracy rates of predicting a flagged alert to a real life event of interest
