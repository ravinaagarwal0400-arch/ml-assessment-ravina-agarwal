PART B — BUSINESS ANSWERS

# B1 - Problem Formulation

B1 (a)-

Target: items_sold
Features: promotion, store size, location, competition, time
Type: Regression

B1 (b)-

-Revenue varies due to pricing
-Items sold is stable

Principle: Choose target variable that directly reflects business objective

B1 (c) - 
-Use store-level models or cluster-based models
-Stores behave differently → segmentation improves accuracy

# B2. Data and EDA Strategy

B2 (a) -

-Join using store_id, date
-Grain: store-month level

B2 (b) - 

EDA ideas:

-Promotion vs sales
-Seasonality trends
-Location performance
-Competition impact

B2 (c) -

-Imbalance → model biased toward “no promotion”
Solution:
-Sampling
-Feature engineering

# B3. Model Evaluation and Deployment

B3 (a) -

-Train: first 2–2.5 years
-Test: last months

Metrics:

-RMSE → penalizes large errors
-MAE → interpretable


B3 (b) -
 - Feature importance shows:
	Seasonality
	Promotion effectiveness


B3 (c) -

Deployment:

-Save model → joblib
-Monthly scoring pipeline
-Monitor:
	Performance drift
	Data drift