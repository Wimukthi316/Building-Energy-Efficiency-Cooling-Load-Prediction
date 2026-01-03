# Building Energy Efficiency - Cooling Load Prediction

> Statistical analysis and predictive modeling of building cooling load requirements based on architectural features

---

## Overview

This project presents a comprehensive statistical analysis of building energy efficiency, focusing on predicting cooling load requirements using multiple building characteristics. The analysis employs various statistical methods including ANOVA, correlation analysis, and linear regression to identify key factors influencing cooling loads.

## Dataset

**Energy Efficiency Dataset (EED.csv)**
- **Observations:** 768 buildings
- **Variables:** 
  - `Surface_Area` - Total surface area (m²)
  - `Wall_Area` - Wall area (m²)
  - `Roof_Area` - Roof area (m²)
  - `Orientation` - Building orientation (categorical)
  - `Cooling_Load` - Cooling load requirement (BTU)

## Methodology

### 1. Descriptive Statistics & Central Tendency

Analysis of distribution patterns using:
- Mean, Median, and Mode calculations
- Standard deviation and variance
- Bell curve visualizations with normal distribution overlay
- Density plots for key variables

**Variables analyzed:**
- Cooling Load
- Surface Area  
- Wall Area
- Roof Area

### 2. Hypothesis Testing

**Research Question:** Does building orientation significantly affect cooling load?

**Statistical Tests:**
- One-way ANOVA (parametric approach)
- Kruskal-Wallis test (non-parametric alternative)
- Tukey HSD post-hoc analysis
- Levene's test for homogeneity of variance

### 3. Correlation & Regression Analysis

**Bivariate Analysis:**
- Pearson/Spearman correlation coefficients
- Simple linear regression models
- Scatter plots with regression lines

**Multiple Regression:**
- Combined predictor model
- R² and adjusted R² evaluation
- Residual diagnostics
- Model validation

## Technical Requirements

```r
install.packages(c("ggplot2", "dplyr", "nortest", "car"))
```

**Libraries:**
- `ggplot2` - Data visualization
- `dplyr` - Data manipulation  
- `nortest` - Normality tests
- `car` - ANOVA and regression diagnostics

## Quick Start

```r
# Run the complete analysis
source("energy_efficiency_analysis.R")
```

Ensure `EED.csv` is in the same directory as the R script.

## Project Structure

```
├── EED.csv                           # Dataset
├── energy_efficiency_analysis.R      # Main analysis script
├── analysis_results.pdf              # Generated report
└── README.md                         # Documentation
```

## Output

The analysis generates:
- Console output with statistical test results
- Multiple visualization plots
- Comprehensive PDF report with all findings
- Model performance metrics

## Key Findings

Results include detailed insights on:
- Distribution characteristics of building variables
- Impact of orientation on cooling requirements
- Strength of relationships between architectural features and cooling load
- Predictive accuracy of regression models

---

**Course:** CSE5014 - Business Analytics  
**Module:** Statistical Analysis & Predictive Modeling
