# 402-Earthquake-ML
Earthquake data obtained from the USGS through Kaggle: https://www.kaggle.com/datasets/shreyasur965/recent-earthquakes

First, we load, clean, and conduct exploratory analysis on 1,137 earthquakes.
We used the Natural Earth vector data to visualize and predict the magnitude of earthquakes using predictor values: 
  felt: Number of people who reported feeling the earthquake.
  cdi: Community Determined Intensity: How strongly was the event felt.
  mmi: Modified Mercalli Intensity, scale used to measure earthquake intensity.
  alert: Alert level (green, yellow, orange, red).

We construct models and test the accuracy of Sci-kit Learn's LinearRegression, RandomForestRegressor, and KNeighboresRegressor. We find optimal parameters and create magnitude predictions based on these parameters.

We also conduct geospatial data analysis using Morran I plots to investigate spatial Autocorrelation, and LISA plots for further visual analysis.

We encounter some problems when trying to create predictive models of when the next large earthquake may happen, specifically because we only track the years 2023 and 2024 earthquakes. That amount of data is not nearly enough to develop an accurate model. Instead, we will use the clustering that Kmeans gave us to look at the average interval between events greater than 1 standard deviation away from the mean. We denote these as significant or more dangerous earthquakes for that region.

Conclusions
Both North America and Alaska have a significant portion of time with no significant events occurring, and a similar effect with the Africa, Europe, and Central Asia region for the latter have of the observation window. South East Asia seems to have more consistent earthquakes with the second highest magnitude threshold at 6.14, while South America has the highest magnitude threshold with more sparse events occurring. This could help response agencies understand patterns in a region's tectonic plate movements. The response frequency and severity should differ between South America and South East Asia due to the differences in the magnitude and frequency of the earthquakes. With more time series data, it may be possible to create forecasting models such as ARIMA for non-seasonal trends like earthquakes.
