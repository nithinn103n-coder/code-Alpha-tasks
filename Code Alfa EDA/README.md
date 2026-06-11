# Exploratory Data Analysis (EDA) - Top Companies Dataset

This repository contains a comprehensive **Exploratory Data Analysis (EDA)** on a dataset containing information about the top 100 companies globally. The analysis covers industry distribution, revenue leaders, geographical concentrations, and data quality checks to extract meaningful business insights.

## 📌 Project Overview
This project is part of a data analysis pipeline (Task 2) aimed at understanding market structures and identifying key trends among dominant companies. Before diving into the data, several critical guiding questions were established:
1. Which industry has the highest number of companies?
2. Which company generates the highest revenue?
3. Is there a relationship between revenue and number of employees?
4. Which headquarters location appears most frequently?
5. Are certain industries dominating the market?
6. Are there any missing or inconsistent values in the dataset?

---

## 📊 Dataset Structure
The dataset (`Companies.csv`) consists of **100 rows** and **6 columns** ($100 	imes 6$). 

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| `Rank` | `int64` | The ranking of the company |
| `Name` | `object` | Name of the company |
| `Industry` | `object` | Primary industry sector |
| `Revenue (USD billions)` | `object` | Annual revenue in billions of USD |
| `Employees` | `object` | Total number of employees |
| `Headquarters` | `object` | Location of the corporate headquarters |

---

## 🛠️ Key Steps & Analysis Performed

### 1. Data Structure Exploration
- Checked the dimensions using `df.shape`.
- Analyzed column features and data types using `df.info()` and `df.dtypes`.

### 2. Data Quality & Cleaning
- **Missing Values:** Checked for completeness using `df.isnull().sum()`. Visualized data integrity with a **Missing Data Heatmap** (`sns.heatmap`), confirming $0\%$ missing data.
- **Duplicates:** Confirmed that there are no duplicate entries in the dataset (`df.duplicated().sum() == 0`).

### 3. Industry-Wise Distribution
- Analyzed the representation of different industries.
- **Financials**, **Retail**, **Technology**, and **Petroleum** emerged as some of the most highly represented industry groups.
- Visualized the counts using a horizontal Seaborn countplot (`sns.countplot`).

### 4. Revenue Leadership Analysis
- Sorted the companies to identify the top 10 revenue-generating companies.
- Visualized leaders using a customized Seaborn barplot (`sns.barplot`).

### 5. Geographical Analysis
- Aggregated company headquarters locations to find major business hubs.
- Plotted the top 10 most frequent headquarters locations.

---

## 🚀 Technologies Used
- **Python 3**
- **Pandas:** For data loading, manipulation, and summary statistics.
- **Matplotlib & Seaborn:** For creating crisp, publication-ready data visualizations (heatmaps, bar plots, and countplots).

---

## 📁 Repository Structure
```bash
.
├── Exploratory Data Analysis (EDA).ipynb  # Main Jupyter Notebook with code & visualizations
├── Companies.csv                           # Input dataset (processed from earlier steps)
└── README.md                              # Project documentation (this file)
```

---

## ⚙️ How to Setup and Run
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/repository-name.git
   cd repository-name
   ```
2. **Install Required Libraries:**
   Make sure you have Python installed, then run:
   ```bash
   pip install pandas matplotlib seaborn notebook
   ```
3. **Launch the Notebook:**
   ```bash
   jupyter notebook "Exploratory Data Analysis (EDA).ipynb"
   ```
4. Run all cells sequentially to reproduce the visual charts and statistical breakdowns.

---

## 📈 Summary of Key Insights
- **Data Completeness:** The dataset is fully clean with zero missing values or duplicate entries, allowing for robust statistical interpretations.
- **Market Dominance:** The **Financials** industry has the highest count of companies among the top 100, closely followed by Retail, Technology, and Petroleum sectors.
- **Hub Concentrations:** Headquarters analysis reveals specific cities and metropolitan areas serve as major global hubs hosting multiple top-tier corporations.
