<div align="center">

# 🏢 Building Energy Efficiency Analysis
### Cooling Load Prediction Using Statistical Modeling

[![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)](https://www.r-project.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)](https://github.com/Wimukthi316/Building-Energy-Efficiency-Cooling-Load-Prediction)

*Advanced statistical analysis and predictive modeling for optimizing building energy efficiency*

[Overview](#-overview) • [Dataset](#-dataset) • [Methodology](#-methodology) • [Installation](#-installation) • [Usage](#-usage)

</div>

---

## 📊 Overview

This project delivers a **comprehensive statistical analysis** of building energy efficiency with a focus on predicting cooling load requirements. Using advanced statistical methods including ANOVA, correlation analysis, and multiple linear regression, the study identifies critical architectural factors that influence cooling loads in buildings.

### 🎯 Project Objectives

- Analyze distribution patterns of key building parameters
- Investigate the impact of building orientation on cooling requirements
- Develop predictive models for cooling load estimation
- Validate findings using both parametric and non-parametric methods

---

## 📁 Dataset

### Energy Efficiency Dataset (EED.csv)

| Feature | Description | Type |
|---------|-------------|------|
| **Surface_Area** | Total surface area of the building | Continuous (m²) |
| **Wall_Area** | Total wall area | Continuous (m²) |
| **Roof_Area** | Total roof area | Continuous (m²) |
| **Orientation** | Building orientation direction | Categorical |
| **Cooling_Load** | Cooling load requirement (Target) | Continuous (BTU) |

> **Sample Size:** 768 observations  
> **Data Quality:** Complete dataset with no missing values

---

## 🔬 Methodology

### 📈 1. Descriptive Statistics & Distribution Analysis

Comprehensive exploration of central tendency and dispersion:

- ✅ **Central Tendency:** Mean, Median, Mode
- ✅ **Dispersion Measures:** Standard Deviation, Variance
- ✅ **Visualizations:** Bell curves with normal distribution overlay
- ✅ **Density Analysis:** Distribution patterns and skewness

**Target Variables:**
- Cooling Load | Surface Area | Wall Area | Roof Area

### 🔍 2. Hypothesis Testing

**Research Question:** *Does building orientation significantly affect cooling load?*

```
H₀: Building orientation has no significant effect on cooling load
H₁: Building orientation significantly affects cooling load
```

**Statistical Methods:**
| Test | Type | Purpose |
|------|------|---------|
| One-way ANOVA | Parametric | Primary hypothesis test |
| Kruskal-Wallis | Non-parametric | Robustness validation |
| Tukey HSD | Post-hoc | Pairwise comparisons |
| Levene's Test | Diagnostic | Variance homogeneity |

### 📉 3. Correlation & Regression Analysis

**Phase 1: Bivariate Analysis**
- Correlation coefficients (Pearson/Spearman)
- Simple linear regression models
- Scatter plots with fitted regression lines
- Residual diagnostics

**Phase 2: Multiple Regression**
- Combined predictor model: `Cooling_Load ~ Surface_Area + Wall_Area + Roof_Area`
- Model evaluation: R², Adjusted R², F-statistic
- Assumption testing: Normality, Linearity, Homoscedasticity
- Cross-validation and performance metrics

---

## 🛠️ Installation

### Prerequisites

```r
# Install required packages
install.packages(c("ggplot2", "dplyr", "nortest", "car"))
```

### Package Overview

| Package | Version | Purpose |
|---------|---------|---------|
| `ggplot2` | Latest | Advanced data visualization |
| `dplyr` | Latest | Data manipulation and transformation |
| `nortest` | Latest | Normality tests (Anderson-Darling, etc.) |
| `car` | Latest | Regression diagnostics and ANOVA |

---

## 🚀 Usage

### Quick Start

```r
# Clone the repository
git clone https://github.com/Wimukthi316/Building-Energy-Efficiency-Cooling-Load-Prediction.git

# Navigate to project directory
setwd("path/to/Building-Energy-Efficiency-Cooling-Load-Prediction")

# Run complete analysis
source("energy_efficiency_analysis.R")
```

### Expected Runtime
⏱️ Approximately 2-3 minutes on standard hardware

---

## 📂 Project Structure

```
Building-Energy-Efficiency-Cooling-Load-Prediction/
│
├── 📄 EED.csv                          # Energy Efficiency Dataset
├── 📜 energy_efficiency_analysis.R     # Main analysis script
├── 📊 analysis_results.pdf             # Comprehensive report
├── 📋 README.md                        # Project documentation
└── 📝 .Rprofile                        # R environment configuration
```

---

## 📤 Output

### Generated Deliverables

| Output Type | Description |
|-------------|-------------|
| 📊 **Visualizations** | Bell curves, scatter plots, box plots, Q-Q plots |
| 📈 **Statistical Reports** | ANOVA tables, regression summaries, correlation matrices |
| 📄 **PDF Report** | Complete analysis with all findings and visualizations |
| 💻 **Console Output** | Detailed test results and model diagnostics |

---

## 🎓 Key Findings

### ✨ Insights

- 📍 **Orientation Impact:** Statistical evidence on how building orientation affects cooling requirements
- 📊 **Predictor Strength:** Identification of most influential architectural features
- 🎯 **Model Performance:** High predictive accuracy with validated regression models
- 📉 **Distribution Patterns:** Detailed characterization of variable distributions

---

## 📜 Academic Context

**Course:** CSE5014 - Business Analytics  
**Focus:** Statistical Analysis & Predictive Modeling  
**Domain:** Energy Efficiency & Sustainable Building Design

---

<div align="center">

### 🌟 Built with Precision • Analyzed with Rigor • Documented with Care

**Made with ❤️ for Data Science**

</div>
