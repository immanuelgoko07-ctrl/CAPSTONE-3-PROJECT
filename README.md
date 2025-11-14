# 📘 **Lifestyle & Sleep Quality Data Analysis — README**

## 📝 **Overview**

This project explores how lifestyle factors such as sleep duration, stress level, physical activity, and BMI influence overall health and well-being. Using Python and Microsoft Excel, the dataset was cleaned, analyzed, and visualized to uncover patterns that affect sleep quality and daily health indicators.

---

## 🎯 **Project Objectives**

* Analyze sleep duration and sleep quality across individuals.
* Examine how stress, physical activity, and BMI affect health outcomes.
* Identify common sleep disorders in the dataset.
* Generate insights that support healthier lifestyle decisions.

---

## 📂 **Dataset Description**

The dataset contains the following key variables:

* **Age**
* **Gender**
* **Occupation**
* **Sleep Duration (hrs)**
* **Quality of Sleep**
* **Stress Level**
* **Physical Activity (mins)**
* **BMI Category**
* **Blood Pressure**
* **Heart Rate (bpm)**
* **Daily Steps**
* **Sleep Disorder**

These variables help assess how daily habits relate to sleep and health.

---

## 🛠️ **Tools & Technologies Used**

* **Python**
* **Pandas** – Data Cleaning & Manipulation
* **Matplotlib** – Data Visualization
* **Seaborn** – Statistical Plotting
* **NumPy** – Numerical Computations
* **Microsoft Excel** – Data Preview, Basic Checks & Exporting
* **Jupyter Notebook / VS Code**

---

## 🔧 **Methods Used**

1. **Data Loading** using Excel and Pandas.
2. **Data Cleaning**, including splitting blood pressure and ensuring numeric types.
3. **Exploratory Data Analysis (EDA)** to understand distributions and patterns.
4. **Visualization** of sleep patterns, stress levels, activity levels, and correlations.
5. **Interpretation of Findings** to derive meaningful insights.

---

## 📊 **Key Visualizations**

* Sleep Duration by Occupation
* Stress vs Sleep Duration Scatter Plot
* Sleep Disorder Distribution
* Heart Rate Boxplot
* Correlation Heatmap

---

## 💡 **Sample Python Code (Loading & Cleaning)**

```python
import pandas as pd

df = pd.read_excel("Lifestyle dataset.xlsx")

# Split Blood Pressure into two columns
df[['Systolic', 'Diastolic']] = df['BloodPressure'].str.split('/', expand=True).astype(int)

df.head()
```

---

## 📈 **Insights**

* Higher stress levels are linked to lower sleep duration and quality.
* Physical activity increases daily steps and supports better heart health.
* Overweight and obese individuals show higher cases of sleep disorders.
* Certain high-pressure occupations have shorter sleep durations.

---

## 🧠 **Conclusion**

The project shows clear relationships between lifestyle behaviors and health outcomes.
By understanding these patterns, individuals can make better-informed choices to improve sleep and overall well-being.

---

## 🚀 **Future Enhancements**

* Add predictive modeling (e.g., predict sleep disorder).
* Create a dynamic dashboard using Plotly or Tableau.
* Expand dataset with lifestyle factors like diet, caffeine, and screen time.

---

## 📁 **Project Structure**

```
Lifestyle-Analysis-Project/
│
├── data/
│   └── lifestyle_dataset.xlsx
│
├── notebooks/
│   └── analysis.ipynb
│
├── scripts/
│   ├── data_cleaning.py
│   └── visualizations.py
│
├── images/
│   └── charts/
│
└── README.md

