# Air Quality Index (AQI) Analysis



## Overview

Air quality index (AQI) analysis is crucial for environmental management and public health. This project presents a comprehensive analysis of the air quality in Delhi during January 2023 using Python. It covers data collection, cleaning, visualization, and interpretation of key metrics.

## Motivation

This project demonstrates how to:
- **Calculate and analyze the Air Quality Index (AQI) based on pollutant concentrations.**
- **Examine the distribution of AQI categories to understand the prevalence of different air quality conditions.** 
- **Investigate hourly trends in AQI to identify patterns and peak pollution hours.** 
- **Explore correlations between different pollutants to assess their relationships.** 
- **Compare the calculated AQI metrics with recommended air quality metrics to evaluate the severity of air quality in Delhi.** 
## Methodology
- **Time series analysis of air pollutants in Delhi**![timeseries](https://github.com/user-attachments/assets/849db0e5-fc87-4578-841c-03a89cde54f8)
- **Calculating AQI**
-  Define AQI breakpoints, corresponding AQI values and AQI categories
aqi_breakpoints = [
    (0, 12.0, 50), (12.1, 35.4, 100), (35.5, 55.4, 150),
    (55.5, 150.4, 200), (150.5, 250.4, 300), (250.5, 350.4, 400),
    (350.5, 500.4, 500)
]
aqi_categories = [
    (0, 50, 'Good'), (51, 100, 'Moderate'), (101, 150, 'Unhealthy for Sensitive Groups'),
    (151, 200, 'Unhealthy'), (201, 300, 'Very Unhealthy'), (301, 500, 'Hazardous')
]

-**Analyzing AQI of Delhi**
  ![aqitre](https://github.com/user-attachments/assets/11e03340-4801-405f-87a2-8ea123681340)![aqicat](https://github.com/user-attachments/assets/850d8a58-cd37-4a8e-9cad-d25ee8b0aad5)![pol](https://github.com/user-attachments/assets/763412ba-bacb-4ae4-99fa-78f86178cab5)
-**Correlation between pollutants**
  ![corrr](https://github.com/user-attachments/assets/326f2de5-7d09-492f-b324-dbc0a26ca756)
  The correlation matrix displayed here represents the correlation coefficients between different air pollutants in the dataset. Correlation coefficients measure the strength and direction of the linear relationship between two variables, with values ranging from -1 to 1. Overall, the positive correlations among CO, NO, NO2, SO2, PM2.5, PM10, and NH3 suggest that they may share common sources or have similar pollution patterns, while O3 exhibits an inverse relationship with the other pollutants, which may be due to its role as both a pollutant and a natural atmospheric oxidant.

-**Hourly average trends of AQI in Delhi**
  ![hrly](https://github.com/user-attachments/assets/74dece21-56cd-49ce-9464-7a76d78d7f31)

-**Average AQI by day of the week in Delhi**
![daily](https://github.com/user-attachments/assets/288a1282-424b-4d17-8e0c-a80d463d7912)

It shows that the air quality in Delhi is worse on Wednesdays and Thursdays.

## Key Insights

- **Pollutant Trends:**  
  Time series analysis reveals distinct fluctuations in pollutants such as CO, NO₂, and PM2.5. Notably, ozone (O₃) shows a different trend compared to other pollutants, reflecting its dual role as both a pollutant and an atmospheric oxidant.

- **AQI Levels:**  
  The computed AQI values predominantly fall within the *Very Unhealthy* to *Hazardous* range, indicating significant air quality issues in Delhi during January 2023.

- **AQI Category Distribution:**  
  Histogram analysis shows the prevalence of hazardous AQI categories, highlighting periods of extreme air quality deterioration.

- **Correlation Among Pollutants:**  
  Strong positive correlations among CO, NO, NO₂, SO₂, PM2.5, and PM10 suggest common sources, while the negative correlation of O₃ with these pollutants provides insights into its unique behavior.

- **Temporal Patterns:**  
  - **Hourly Trends:** AQI peaks during certain hours, suggesting a strong link with daily human activities and meteorological conditions.  
  - **Weekly Trends:** The analysis indicates that air quality worsens on mid-week days (Wednesday and Thursday), potentially due to increased vehicular and industrial activities.

## Conclusion

This project demonstrates how to perform in-depth AQI analysis using Python. The results provide valuable insights into pollutant trends and air quality patterns in Delhi, which can inform environmental policy and public health decisions.
