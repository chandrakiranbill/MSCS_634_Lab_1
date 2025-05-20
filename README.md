# MSCS_634_Lab_1
2025 Summer - Advanced Big Data and Data Mining

# MSCS 634 – Lab 1: Data Visualization, Preprocessing, and Statistical Analysis

## Student Name:
Chandra Kiran Billingi


## Lab Title:
Lab 1 : Data Visualization, Data Preprocessing, and Statistical Analysis Using Python 

---

##  Purpose of the Lab

The objective of this lab was to apply foundational data science techniques including data visualization, preprocessing, and statistical analysis using Jupyter Notebook. By using a real-world weather dataset from Austin, TX, I explored trends, cleaned the data, handled missing values and outliers, scaled and discretized numerical features, and performed descriptive statistics to better understand the dataset.

---

## 📊 Key Insights

### Data Visualization
- **Line Plot** showed seasonal temperature trends across the year, revealing clear temperature cycles.
- **Histogram** of humidity levels illustrated that most days had high humidity, especially in the summer.
- **Scatter Plot** between temperature and dew point showed a strong positive correlation.

### Data Preprocessing
- Replaced placeholder characters (`'O'`, `'-'`) with missing values (`NaN`) and then imputed them using mean/mode strategies.
- Removed outliers using the IQR method, especially from wind and visibility columns.
- Dropped irrelevant or redundant features and sampled the data to reduce dimensionality.
- Applied **Min-Max Scaling** to normalize features like temperature, humidity, and wind speed.
- **Discretized** scaled features into "Low", "Medium", and "High" bins for categorical analysis.

### Statistical Analysis
- **Central Tendency**: Mean and median were closely aligned for most features, indicating symmetric distributions.
- **Dispersion**: Features like wind speed had higher standard deviation and range, while humidity was more consistent.
- **Correlation Matrix**: Strong positive correlation between temperature and dew point; weak or negative correlation between wind speed and pressure.

---

## ⚠️ Challenges & Decisions

- The original dataset contained formatting inconsistencies (`'T'`, `'0.00'`, `'-'`), which required custom replacement and data type correction.
- Some features like `'PrecipitationSumInches'` contained `'T'` for trace values. These were left untouched to preserve meteorological meaning.
- Deciding the appropriate bins for discretization required evaluating distribution histograms.
- I chose Min-Max Scaling for normalization due to its bounded [0, 1] output, which is ideal for visual clarity and comparability.

---



