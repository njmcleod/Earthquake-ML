# 402-Earthquake-ML
Earthquake data obtained from the USGS through Kaggle: https://www.kaggle.com/datasets/shreyasur965/recent-earthquakes

First, we load, clean, and conduct exploratory analysis on 1,137 earthquakes.
We used the Natural Earth vector data to visualize and predict the magnitude of earthquakes using predictor values: 
  felt: Number of people who reported feeling the earthquake.
  cdi: Community Determined Intensity: How strongly was the event felt.
  mmi: Modified Mercalli Intensity, scale used to measure earthquake intensity.
  alert: Alert level (green, yellow, orange, red).

We construct models and test the accuracy of Sci-kit Learn's LinearRegression, RandomForestRegressor, and KNeighboresRegressor. We find optimal parameters and create magnitude predictions based on these parameters.


