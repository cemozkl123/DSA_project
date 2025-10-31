# 🌦️ Weather-and-Air-Quality-in-Istanbul

## 💡 *Project Idea*

This project aims to investigate the relationship between **weather conditions** (temperature, rainfall, humidity) and **air quality metrics** (PM2.5, PM10, NO₂, SO₂, CO, O₃) in **Istanbul, Türkiye**.  
I hypothesize that rainy and humid days will show **lower particulate pollution levels** due to atmospheric cleansing effects, while dry and stagnant conditions will correspond to **higher pollutant concentrations**.  

By analyzing daily weather and air quality data from 2024, this project seeks to **quantify how weather patterns influence Istanbul’s air quality** and identify which meteorological variables most strongly correlate with pollution levels.

---

## 💭 *Motivation*

Living and studying at **Sabancı University**, I have personally noticed that the **air quality is often poor**, especially during dry or stagnant weather conditions.  
This observation made me wonder: 💡 *does rain actually help clean the air and improve air quality around us?*  
With Istanbul being one of Türkiye’s most populated and industrially active cities, the link between **weather and pollution** felt like an important question to explore.  
This project aims to investigate whether **rainfall and humidity** play a measurable role in reducing air pollution — and how weather patterns shape the environmental conditions we live in every day.

---

## 📊 *Description of Datasets*
The project will utilize two primary datasets:

### ☁️ *Weather Dataset*
- **Source:** [Meteostat](https://meteostat.net/en/place/tr/istanbul)  
- **Description:** Historical daily weather data for Istanbul in 2024.  
- **Key Features:**  
  - 📅 `Date`: Daily timestamps  
  - 🌡️ `Temperature (°C)`: Average daily temperature  
  - 💧 `Humidity (%)`: Average daily humidity level  
  - 🌧️ `Precipitation (mm)`: Rainfall volume  
  - ⛅ `Conditions`: Weather status (e.g., Clear, Rain, Cloudy)  

---

### 🌫️ *Air Quality Dataset*
- **Source:** [Kaggle – Marmara Air Quality Data Analysis 2024: Insights from Istanbul Kandilli](https://www.kaggle.com/datasets)  
- **Description:** Hourly air pollutant measurements recorded at the Kandilli monitoring station in Istanbul, aggregated into daily averages.  
- **Key Features:**  
  - 📅 `Date`: Measurement date  
  - 🫧 `PM2.5`, `PM10`: Particulate matter concentrations  
  - 🧪 `NO₂`, `SO₂`, `CO`, `O₃`: Gas pollutant levels  
  - 📍 `Station Name`: Monitoring location (Kandilli)  

---

## 🧩 *Plan*

### 🗂️ *Data Collection*
- *Weather Data Source:*  
  - Meteostat — Historical daily weather data (2024)  
- *Air Quality Data Source:*  
  - Kaggle — Marmara Air Quality Dataset (2024, Istanbul Kandilli)

---

### 🔍 *Data Analysis Approach*

1. 🧭 *Exploratory Data Analysis*  
   - Plot daily temperature, humidity, and rainfall distributions  
   - Visualize pollutant level trends throughout 2024  
   - Compare pollutant concentrations on rainy vs. clear days  

2. 📈 *Statistical Analysis*  
   - Correlation matrix between weather and pollutant variables  
   - Regression models to identify which weather factors predict air quality changes  
   - Hypothesis testing to assess the significance of rainfall effects  

3. 🎨 *Visualization and Presentation*  
   - Time-series graphs for weather and air pollutant trends  
   - Heatmaps showing weather-pollutant relationships  
   - Scatter plots comparing precipitation and particulate matter levels  

---

### 🛠️ *Tools and Technologies*
- 🐍 *Python*: Main programming language  
- 📦 *Pandas & NumPy*: Data cleaning and manipulation  
- 📊 *Matplotlib & Seaborn*: Visualization and correlation analysis  
- 🤖 *Scikit-learn*: Regression and predictive modeling  

---

## 🎯 *Expected Outcomes*
- Identification of statistically significant correlations between weather variables and pollution metrics.  
- Quantitative evidence showing **rain and humidity reduce PM2.5 and PM10 levels** in Istanbul.  
- Visual representations of how weather affects air quality over time.  
- A simple regression-based predictive framework for estimating pollutant levels using meteorological variables.  
- Insights that can support **urban air quality management and environmental awareness**.  

---

## 🧠 *Future Plans*
Based on the findings from this study, in the future i can:  
- 🛰️ Develop a **predictive model** that estimates daily air pollution levels using real-time weather data.  
- 📅 Extend the analysis across multiple years to observe long-term environmental trends.  
- 🌍 Compare Istanbul’s findings with other major Turkish cities such as Ankara or Izmir.  
- 💻 Build an interactive **data visualization dashboard** that forecasts pollution conditions based on weather forecasts.  

These advancements could help citizens, policymakers, and environmental organizations better understand — and even **anticipate** — how weather influences the air we breathe.

---

## ⚠️ *Potential Challenges*
- Missing or inconsistent hourly records in air quality data.  
- Variability in measurement accuracy across monitoring periods.  
- Limited generalizability since data represents a single monitoring station (Kandilli).  
- Distinguishing correlation from causation — weather may influence but not directly cause air quality changes.  

---

🌍 This project will contribute valuable insights into how weather conditions affect air pollution in Istanbul.  
The findings could inform **public health awareness**, **environmental planning**, and **data-driven pollution mitigation strategies** for urban environments.
