🌦️ Weather and Air Quality in Istanbul
📘 Overview

This project investigates the relationship between weather conditions and air quality in Istanbul, Türkiye.
Specifically, it explores how variables such as rainfall, humidity, and temperature influence air pollutants like PM2.5 and PM10.

The project is prepared for DSA210: Introduction to Data Science (Fall 2025–2026), and it follows the complete data science process — from data collection and cleaning to analysis, visualization, and interpretation.

🎯 Motivation

Air pollution is a growing concern in Istanbul due to rapid urbanization, industrial activity, and high traffic density. Weather factors like rain and wind play a crucial role in dispersing or washing away pollutants.

Through this project, we aim to:

Examine how rainy and dry weather conditions impact air quality levels.

Identify which meteorological variables most strongly correlate with changes in air pollution.

Provide data-driven insights that may support environmental policy and public health initiatives.

💾 Data Sources
1️⃣ Weather Data (Istanbul, 2024)

Source: Meteostat

Description: Historical daily weather data for Istanbul for the year 2024.

Features:

Date — Daily record date

Temperature (°C)

Precipitation (mm)

Humidity (%)

Conditions (Clear, Rain, Cloudy, etc.)

Purpose: Identify rainy days and measure variations in temperature and humidity to evaluate their effects on air pollution.

2️⃣ Air Quality Data (Istanbul – Kandilli, 2024)

Source: Kaggle – Marmara Air Quality Data Analysis 2024: Insights from Istanbul Kandilli

Description: Hourly air quality measurements from the Kandilli monitoring station in Istanbul.

Features:

Date

PM10, PM25, NO2, SO2, CO, O3

Purpose: Evaluate daily air pollution levels and correlate them with weather variables such as rainfall and humidity.

🔍 Research Questions

Does rainfall significantly reduce PM2.5 and PM10 levels in Istanbul?

Which weather factors (temperature, humidity, wind, rain) most strongly affect air pollutant concentrations?

Are there identifiable seasonal or monthly trends linking weather patterns to air quality changes?

🧠 Methodology

Data Collection

Weather data retrieved from Meteostat (2024 daily dataset).

Air quality data downloaded from Kaggle (Kandilli station, hourly readings).

Data Cleaning

Convert time formats to datetime.

Aggregate hourly air quality readings into daily averages.

Handle missing or inconsistent records.

Standardize variable names across datasets.

Merging

Merge weather and air quality datasets using the Date column.

Create a binary variable Rainy (1 = rainy day, 0 = clear day).

Analysis

Perform correlation analysis between weather and pollutant variables.

Conduct statistical hypothesis testing (e.g., t-tests).

Explore predictive relationships using simple regression models.

Visualization

Time-series plots of temperature, rainfall, and pollutant trends.

Heatmaps showing correlation between weather and pollution variables.

Scatter plots illustrating rain’s effect on particulate matter.

📊 Expected Outcomes

Clear correlation patterns between rainfall and lower particulate pollution.

Insights into how Istanbul’s 2024 weather conditions influenced air quality.

Visual evidence supporting the hypothesis that rain and humidity improve air quality.

Potential use for forecasting pollution based on weather patterns.

⚙️ Tools and Technologies
Category	Tools
Programming	Python
Libraries	pandas, numpy, matplotlib, seaborn, scikit-learn
Platform	Jupyter Notebook / Google Colab
Version Control	Git & GitHub
🚧 Limitations and Future Work

Air quality data is limited to one station (Kandilli) — results may not generalize citywide.

Some missing or uneven hourly readings may introduce bias.

Future improvements may include:

Expanding to multiple air quality stations across Istanbul.

Including wind speed and direction for more precise models.

Applying time-series forecasting to predict pollution trends.
