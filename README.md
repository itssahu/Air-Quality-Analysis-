# Air Quality Index (AQI) Analysis Using Python

![AQI Banner](images/aqi_bar_chart.png)

## Overview

Air quality index (AQI) analysis is crucial for environmental management and public health. This project presents a comprehensive analysis of the air quality in Delhi during January 2023 using Python. It covers data collection, cleaning, visualization, and interpretation of key metrics.

## Motivation

With rising urbanization, air quality has become a pressing issue. This project demonstrates how to:
- **Gather and preprocess** air quality data from various sources.
- **Calculate AQI** using standardized formulas.
- **Visualize** pollutant trends over time.
- **Extract insights** to help understand pollution patterns and inform policy decisions.

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

## Repository Contents

- **Data:**  
  The dataset `delhiaqi.csv` contains hourly measurements of various pollutants in Delhi during January 2023.

- **Notebooks:**  
  The `AQI_Analysis.ipynb` notebook walks through the analysis step-by-step, including data cleaning, visualization, and AQI calculation.

- **Scripts:**  
  The `aqi_analysis.py` script provides a standalone version of the analysis, which can be executed to reproduce the results.

- **Images:**  
  Sample plots and visualizations (time series, bar charts, donut charts, correlation heatmaps, etc.) are stored in the `images/` folder.

## How to Run the Project

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/air-quality-index-analysis.git
   cd air-quality-index-analysis
