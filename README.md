# Nigeria Health Data Analysis

This project offers a detailed analysis of health-related statistics for Nigeria, focusing on causes of death, public health indicators, and national health targets. The analysis is built from data scraped from the [World Health Organization (WHO)](https://www.who.int/) website, compiled into the `Nigeria.xlsx` file, and paired with insights from a supplementary report (`Nigeria.pdf`).

---

## Data Sources

- **Nigeria.xlsx**: Contains scraped health data from WHO including:
  - Population statistics (current & projected)
  - Causes of death and associated death rates
  - Health statistics and corresponding targets

- **Nigeria.pdf**: Provides summarized visual insights, statistics, and breakdowns that support the spreadsheet data.

---

## Analysis Objectives

This project investigates:
- Major causes of death and their relative contribution to mortality
- Relationship between population metrics and death rates
- Key health statistics vs. national targets
- Distribution and anomalies in death rate data

---

## Key Findings

### Top Causes of Death
| Cause                         | Death Rate |
|------------------------------|------------|
| Malaria                      | 83.5       |
| Lower respiratory infections | 83.3       |
| Diarrhoeal diseases          | 64.0       |
| Tuberculosis                 | 55.9       |
| Maternal conditions          | 45.4       |

**Contribution to Total Death Rate (515.00):**
- Lower respiratory infections — 36.04%
- Diarrhoeal diseases — 27.13%
- Malaria — 16.47%
- Tuberculosis — 11.55%
- Maternal conditions — 8.82%

### Death Rate Statistics

| Metric             | Value   |
|--------------------|---------|
| Total Death Rate   | 515.00  |
| Average Death Rate | 73.57   |
| Max Death Rate     | 95.90   |
| Min Death Rate     | 45.40   |

---

## Exploratory Data Analysis

### Population Metrics
- Current and projected population fields were sparsely populated and partially non-numeric.
- Death rate correlations with population metrics were visualized and tested.

### Health Statistics & Targets
- Health statistics were extracted and compared to stated health targets.
- Relationships between statistics and goals were visualized through bar plots.

### Distribution & Outliers
- Death rates were examined using histograms, KDE plots, and boxplots.
- Outlier detection was applied using IQR-based filtering.

---

## Project Dependencies

Install required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn
