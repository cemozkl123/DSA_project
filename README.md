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

## 📌 Phase 2 — Data Cleaning, Integration, and Exploratory Analysis

### 🎯 Objective
The goal of Phase 2 was to prepare and explore the weather and air quality datasets by cleaning, integrating, and analyzing them to uncover initial relationships between meteorological conditions and air pollution levels in Istanbul.

---

### 🛠️ What We Did
- Cleaned and preprocessed both weather and air quality datasets
- Converted date fields into a consistent daily format
- Aggregated hourly air quality measurements into daily averages
- Handled missing and inconsistent data entries
- Merged weather and air quality datasets based on date
- Created a unified daily dataset for Istanbul (2024)
- Saved the cleaned and merged dataset for further analysis in Phase 3

---

### 📊 Exploratory Data Analysis
- Visualized daily trends of temperature, humidity, precipitation, and pollutants
- Compared air pollution levels on rainy versus non-rainy days
- Analyzed seasonal variations in particulate matter and gaseous pollutants
- Examined distributions and temporal patterns of PM2.5 and PM10

---

### 🔍 Key Findings
- Rainy days generally exhibit lower PM2.5 and PM10 concentrations, supporting the atmospheric cleansing hypothesis
- Dry and stagnant weather conditions are associated with higher pollution levels
- Certain pollutants display seasonal trends, indicating meteorological influence
- Weather variables appear to play a meaningful role in short-term air quality fluctuations

---

### 💡 Insights & Lessons Learned
Phase 2 demonstrated the importance of proper data cleaning and alignment when working with multi-source environmental data. The exploratory analysis provided early evidence supporting the hypothesis that weather conditions—particularly precipitation and humidity—affect air quality in Istanbul, motivating deeper statistical and predictive analysis in Phase 3.

## 📌 Phase 3 — Modeling and Interpretation

### 🎯 Objective
The goal of Phase 3 was to quantitatively model the relationship between meteorological variables and air pollution levels. Using the cleaned dataset from Phase 2, multiple regression-based models were evaluated to determine which approach best captures the relationship between weather conditions and PM10 concentration.

---

### 🛠️ What We Did
- Loaded the merged daily dataset created in Phase 2
- Selected key meteorological features including temperature, humidity, and precipitation
- Trained multiple models to predict PM10 concentration
- Evaluated model performance using RMSE and R² metrics
- Compared linear and non-linear modeling approaches

---

### 🏆 Best Performing Model
Among the evaluated models, **Random Forest Regression** achieved the **lowest RMSE** and the **highest R² score**, indicating superior predictive performance compared to linear models.

The improved performance of Random Forest suggests that the relationship between meteorological variables and PM10 concentration is **non-linear** and cannot be fully captured using simple linear assumptions.

---

### 📊 Key Results
- Random Forest outperformed Linear Regression in both error reduction and explanatory power
- Precipitation and humidity are strongly associated with lower PM10 concentrations
- Temperature shows a weaker and less consistent influence
- Non-linear interactions between weather variables appear to play an important role in pollution dynamics

---

### 🔍 Interpretation
The results indicate that weather conditions influence air quality in a complex, non-linear manner. While linear models provide a useful baseline, Random Forest better captures interactions and threshold effects present in the data.

---

### 💡 Insights & Lessons Learned
Phase 3 highlights the importance of selecting models that match the structure of the data. For this dataset, Random Forest proved to be the most effective approach by capturing non-linear relationships between meteorological factors and PM10 levels, resulting in more accurate predictions.

