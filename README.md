# Nigeria Health Data Analysis

This repository presents an extensive data-driven analysis of Nigeria's public health landscape, focusing on causes of death, health statistics, and national health targets. The project integrates structured data scraped from the [World Health Organization (WHO)] website and is supplemented by key insights extracted from the **Nigeria Health Report (Nigeria.pdf)**.

---

## Data Overview

- **Source**: Scraped from WHO’s publicly available datasets.
- **Primary File**: `Nigeria.xlsx`
- **Supplementary Document**: `Nigeria.pdf` summarizing mortality trends and demographic health patterns.

### Dataset Features:
- Current & Projected Population figures
- Leading causes of death and associated death rates
- National health statistics and corresponding target values

---

## Objectives

This project aims to:
- Identify top contributors to mortality rates in Nigeria
- Analyze relationships between population dynamics and death rates
- Compare health indicators against target benchmarks
- Detect patterns, outliers, and visualize health trends across regions

---

## Key Findings

### Mortality Insights

| Cause of Death                  | Death Rate | Contribution to Total (%) |
|--------------------------------|------------|----------------------------|
| Lower respiratory infections   | 83.3       | 36.04%                     |
| Malaria                        | 83.5       | 16.47%                     |
| Diarrhoeal diseases            | 64.0       | 27.13%                     |
| Tuberculosis                   | 55.9       | 11.55%                     |
| Maternal conditions            | 45.4       | 8.82%                      |

**Overall Death Metrics from PDF Report:**

- **Total Death Rate**: 515.00  
- **Average Death Rate**: 73.57  
- **Maximum Death Rate**: 95.90  
- **Minimum Death Rate**: 45.40  

### Population Context

- Population fields are partially descriptive and non-numeric.
- Visual map (from `Nigeria.pdf`) highlights regions with lowest projected population floors.
- Additional projections:
  - Healthier Populations: ~54.3m (37.6m – 69.5m)
  - Universal Health Coverage: ~14.9m (9.3m – 20.7m)
  - Health Emergency Protection: ~7.7m (−34m – 49.1m)

### Health Statistics vs Targets

Sample health metrics include:
- Maternal Mortality: 1,000 per year
- Neonatal Mortality: 34.3
- Air Pollution Mortality: 175
- Under-5 stunting: 11.6%
- Hypertension: 36.1%
- Tobacco use: 3.3%
- Clean fuels access: 24.4%
- Domestic government health expenditure: 4.3%

Target alignment and gaps are visualized using bar charts.

---

## Technology & Tools

### Programming Language:
- Python (Jupyter Notebook / Google Colab)

### Key Libraries:
```bash
pip install pandas numpy matplotlib seaborn
Imports:
python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
 Data Preprocessing
Basic operations performed:

Fill missing values: df_filled = df.fillna(0)

Shape: (72 rows, 8 columns)

Data sampling and descriptive statistics

Unique checks on categorical fields

Type coercion to support numeric operations

 Exploratory Data Analysis

Major analytical tasks:

Grouping & ranking causes of death by average death rate

Identifying and removing non-informative entries

Visualizing death rate distribution using histograms, KDE & boxplots

Checking outliers via IQR methodology

Scatter plots to compare population metrics with death rates

 Visual Highlights
Bar Charts: Death rates by cause

Scatter Plots: Population vs death rate correlations

Boxplots: Outlier detection

Histogram + KDE: Death rate distribution

Categorical Frequency Plots: Health targets by type

 Conclusion

This project offers a clear data-centric narrative about
 Nigeria’s public health trends and challenges.

It surfaces critical insights on preventable mortality,
 healthcare access, and government health priorities.

The fusion of scraped numerical data and descriptive
 health report enhances the depth and reliability
of findings, providing stakeholders, students,
and policymakers with actionable information.

 Repository Contents
 Nigeria-Mortality-Stats/
│
├── Nigeria.xlsx            # Structured health dataset
├── Nigeria.pdf             # Health insights summary report
├── Nigeria_Health.ipynb    # Analysis notebook
└── README.md               # This documentation
