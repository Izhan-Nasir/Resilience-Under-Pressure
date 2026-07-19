# Resilience Under Pressure
### A Data-Driven Framework for Global Disaster Risk, Response, and Recovery Analytics

An end-to-end data analytics project that quantifies disaster resilience across countries by integrating humanitarian, economic, and governance datasets into a unified analytical platform.

This project combines data engineering, feature engineering, statistical modeling, and interactive Tableau dashboards to transform raw global datasets into actionable resilience metrics for policy and humanitarian decision-making.

---

## Project Overview

Natural disasters are inevitable, but their impact depends heavily on a country's economic strength, governance, and adaptive capacity.

This project develops a comprehensive analytical framework that measures resilience using publicly available datasets from:

- EM-DAT International Disaster Database
- World Bank World Development Indicators (WDI/WGI)
- United Nations Development Programme (UNDP)

The final output is an interactive Tableau dashboard that enables comparative analysis of disaster vulnerability, recovery capacity, and long-term resilience across countries.

---

## Objectives

- Integrate heterogeneous global datasets into a unified analytical pipeline
- Design quantitative metrics for disaster resilience
- Engineer meaningful features from socio-economic indicators
- Analyze recovery trends across nearly three decades
- Build interactive dashboards for decision-makers

---

# Tech Stack

### Languages

- Python

### Libraries

- Pandas
- NumPy

### Visualization

- Tableau

### Data Sources

- EM-DAT
- World Bank (WDI/WGI)
- UNDP

---

# Dataset Pipeline

```
EM-DAT
            \
             \
              ---> Data Cleaning
World Bank    ---> Missing Value Handling
              ---> Feature Engineering
UNDP          ---> Data Fusion
                     |
                     ▼
             Composite Indices
                     |
                     ▼
          Tableau Interactive Dashboard
```

---

# Data Engineering

The project required extensive preprocessing before any analysis could be performed.

### Data Cleaning

- Merged multiple datasets using Country-Year keys
- Aggregated event-level disaster records
- Removed inconsistent records
- Standardized country identifiers

### Missing Value Strategy

Implemented different imputation strategies depending on variable type:

**Structural Variables**

- GDP
- Population
- HDI
- Infrastructure

Methods:
- Linear interpolation
- Forward filling

**Event Variables**

- Fatalities
- Affected population
- Disaster count

Methods:
- No interpolation
- Missing disaster records treated as zero events

---

# Feature Engineering

Several new variables were engineered for meaningful comparison.

### Per-Capita Metrics

- Fatalities per million
- Population affected (%)

### Transformations

- Log Transformation
- Min-Max Normalization

### Derived Features

- GDP Growth
- Disaster Frequency
- Average Disaster Severity
- Adaptive Capacity

---

# Analytical Models

## 1. Disaster Impact Index (DII)

Measures disaster severity relative to a country's economic capacity.

Considers:

- Fatalities
- Population affected
- GDP
- Disaster severity

---

## 2. Resilience Recovery Score (RRS)

Evaluates how quickly a country recovers economically after disasters.

Factors include:

- GDP recovery time
- Human Development Index
- Political Stability

Implemented using a custom look-ahead recovery algorithm.

---

## 3. Composite Resilience Index (CRI)

A holistic resilience metric based on:

- Adaptive Capacity
- Exposure
- Vulnerability

This serves as the primary resilience indicator throughout the dashboard.

---

# Dashboard Highlights

The Tableau dashboard consists of three analytical sections.

## Global Vulnerability & Development

Explores:

- Human Development Index
- Vulnerability Score
- Global resilience gap
- Geographic disparities

---

## Economic Capacity & Recovery

Analyzes:

- GDP vs Recovery
- Wealth-resilience correlation
- Disaster recovery performance
- Economic resilience

---

## Governance & Adaptive Capacity

Visualizes relationships between:

- Political Stability
- Adaptive Capacity
- Life Expectancy
- Long-term resilience

---

# Key Insights

- Wealth significantly improves disaster resilience.
- Political stability strongly correlates with recovery capacity.
- Infrastructure investments improve both disaster preparedness and public health.
- Many developing countries remain trapped in high-risk recovery cycles despite gradual economic growth.

---

# Skills Demonstrated

- Data Cleaning
- ETL
- Data Wrangling
- Data Fusion
- Feature Engineering
- Missing Value Imputation
- Statistical Analysis
- Exploratory Data Analysis (EDA)
- Composite Index Design
- Tableau Dashboard Development
- Data Visualization
- Analytical Storytelling
- Research Methodology

---

# Author

**Izhan Nasir**

FAST National University of Computer & Emerging Sciences (FAST-NUCES)

Department of Data Science

---


