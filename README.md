# 🚀 5-Minute Data Analysis with YData Profiling

## 📊 Project Overview

This project demonstrates how to perform **automated Exploratory Data Analysis (EDA)** in Python within just a few minutes using the **YData Profiling** library.

For this project, I analyzed a **FIFA World Cup 2026 Player Performance** dataset and generated an interactive HTML profiling report containing important statistical and data-quality insights.

The generated report uses **YData Profiling v4.18.1**.

---

## 🎯 Project Objective

The main objective is to understand a dataset quickly without manually performing every EDA step.

Instead of writing separate code for:

- Dataset overview
- Missing-value analysis
- Statistical summary
- Data-type analysis
- Duplicate detection
- Distribution analysis
- Correlation analysis
- Data-quality checks

YData Profiling automatically generates these insights in a single interactive report.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **YData Profiling**
- **Jupyter Notebook**
- **HTML**

---

## 📁 Dataset

### FIFA World Cup 2026 Player Performance

The project uses a FIFA World Cup 2026 player-performance dataset.

The analysis focuses on automatically understanding the structure, quality, and statistical characteristics of the player-performance data.

---

## ⚡ How It Works

The workflow is very simple:

```text
Dataset
   ↓
Load Dataset using Pandas
   ↓
Create YData Profiling Report
   ↓
Generate Interactive HTML Report
   ↓
Explore Dataset Insights
```

---

## 💻 Installation

Install the required libraries:

```bash
pip install pandas ydata-profiling
```

---

## 🧑‍💻 Python Code

```python
import pandas as pd
from ydata_profiling import ProfileReport

# Load dataset
df = pd.read_csv("fifa_world_cup_2026_player_performance.csv")

# Generate profiling report
profile = ProfileReport(
    df,
    title="FIFA World Cup 2026 Player Performance Analysis",
    explorative=True
)

# Export report
profile.to_file("fifa_world_cup_2026_player_performance_report.html")

print("Report generated successfully!")
```

---

## 📊 What the Report Provides

The automated report helps analyze:

### 1. Dataset Overview
- Number of observations
- Number of variables
- Data types
- Dataset structure

### 2. Variable Analysis
- Numerical variables
- Categorical variables
- Unique values
- Missing values

### 3. Data Quality
- Missing data
- Duplicate records
- Constant values
- Potentially problematic variables

### 4. Statistical Analysis
- Mean
- Median
- Minimum
- Maximum
- Standard deviation
- Quantiles

### 5. Visualization

YData Profiling automatically creates visual insights such as:

- Histograms
- Variable distributions
- Correlation analysis
- Missing-value information

---

## 📄 Project Files

```text
5-Minute-Data-Analysis-with-YData-Profiling/
│
├── fifa_world_cup_2026_player_performance.csv
├── fifa_world_cup_2026_player_performance_report.html
├── analysis.ipynb
└── README.md
```

---

## ⏱️ Why This Project?

Traditional EDA can require many lines of code and several manual steps.

With YData Profiling, a large portion of the initial dataset investigation can be automated, allowing analysts to quickly identify:

**"What is inside my dataset?"**

before moving toward deeper analysis and visualization.

---

## 💡 Key Learning

Through this project, I learned how to:

- Automate EDA using Python
- Generate interactive data-analysis reports
- Identify missing and duplicate data
- Understand variable distributions
- Explore correlations
- Perform initial data-quality checks
- Use Python libraries to reduce repetitive analysis work

---

## 🔮 Future Improvements

I plan to extend this project by adding:

- Data cleaning
- Advanced statistical analysis
- Data visualization using Matplotlib and Seaborn
- Power BI dashboard
- Player-performance insights
- Machine Learning analysis

---

## 👨‍💻 Author

**Abhishek Tyagi**

MCA | Aspiring Data Analyst / Data Scientist

### Skills

`Python` • `Pandas` • `SQL` • `Excel` • `Power BI` • `Data Analysis` • `EDA`

---

⭐ If you find this project useful, consider giving the repository a **star**!
