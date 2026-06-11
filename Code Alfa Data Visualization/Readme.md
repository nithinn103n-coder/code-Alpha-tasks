# Data Visualization - Top Global Companies Analysis

This repository contains a structured data visualization pipeline (**Task 3**) built to extract graphical insights from a dataset detailing the top 100 global companies. By leveraging statistical plotting tools, this project illustrates market distributions, financial hierarchies, corporate staffing balances, and structural anomalies.

---

## 📌 Project Overview
Following the exploratory phase, this section of the workflow is fully dedicated to advanced data visualization. The graphics are meticulously crafted to translate raw numerical data into publication-ready business insights. 

Key visualization targets include:
1. **Revenue Distribution:** Inspecting skewness and data density across the corporate spectrum.
2. **Employees Boxplot:** Identifying global workforce distributions and staffing outliers.
3. **Employees vs. Revenue Correlation:** Mapping how organizational size reflects on raw market performance.
4. **Top Industry Distribution:** Gauging overall market composition among sector leaders.

---

## 📊 Source Dataset Reference
The pipeline visualizes properties extracted from `Companies.csv`. The primary structure maps to the following dimensions:

| Column Name | Sample Row 1 (`Walmart`) | Sample Row 2 (`Amazon`) | Primary Data Focus |
|:---|:---|:---|:---|
| **Rank** | `1` | `2` | Global corporate echelon |
| **Name** | `Walmart` | `Amazon` | Corporate Identity |
| **Industry** | `Retail` | `Retail and cloud computing` | Structural Segment |
| **Revenue (USD billions)**| `6,80,985` | `6,37,959` | Raw Performance Metric |
| **Employees** | `5.10%` | `11.00%` | Operational workforce load |
| **Headquarters** | `21,00,000` | `15,56,000` | Administrative Location |

---

## 🛠️ Visualizations Pack Implementation

The project relies on a comprehensive multi-subplot Matplotlib framework to deliver data summaries cleanly in a single window view.

### Key Plot Components Built:
* **Histogram with KDE (`sns.histplot`):** Evaluates clean density estimations of corporate earnings across all 100 listings.
* **Boxplot Distribution (`sns.boxplot`):** Isolates central quartiles of active workforce sizes and surfaces outlying payroll structures.
* **Scatter Matrix Mapping (`sns.scatterplot`):** Intersects company staffing volumes against revenue outputs to study macro productivity and economies of scale.
* **Categorical Bar Charts (`kind='bar'`):** Aggregates cross-industry volume to identify the top 5 dominating sectors, with axes configurations optimized at a 45-degree rotation for layout clarity.

---

## 🚀 Core Technologies
* **Python 3**
* **Pandas:** Tabular parsing and high-performance dataframe slicing.
* **Matplotlib (Pyplot):** Base canvas configuration and customized axis orientation controls.
* **Seaborn:** Statistical color palettes, Kernel Density Estimations (KDE), and distribution modeling.

---

## 📁 Project Directory
```bash
.
├── Data Visualization.ipynb               # Subplot orchestration & visualization rendering
├── outputs/
│   └── Companies.csv                       # Curated industrial reference dataset
└── README.md                               # Project documentation