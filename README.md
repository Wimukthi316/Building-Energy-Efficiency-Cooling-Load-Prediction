# Building Energy Efficiency - Cooling Load Prediction

Statistical analysis of building energy efficiency data to predict cooling load requirements based on building characteristics.

## Dataset

Energy Efficiency Dataset (EED.csv) containing 768 observations with building parameters including:
- Surface Area
- Wall Area
- Roof Area
- Building Orientation
- Cooling Load (target variable)

## Analysis Components

### 1. Central Tendency Analysis
Distribution analysis with bell curves for:
- Cooling Load
- Surface Area
- Wall Area
- Roof Area

### 2. Hypothesis Testing
ANOVA analysis to test the effect of building orientation on cooling load, including:
- Parametric tests (ANOVA)
- Non-parametric alternatives (Kruskal-Wallis)
- Post-hoc pairwise comparisons

### 3. Correlation and Regression Analysis
- Individual correlation tests between cooling load and building features
- Simple linear regression models
- Multiple linear regression for combined predictors
- Model diagnostics and validation

## Requirements

```r
ggplot2
dplyr
nortest
car
```

## Usage

```r
source("energy_efficiency_analysis.R")
```

## Results

Analysis outputs include:
- Statistical summaries and hypothesis test results
- Distribution visualizations
- Regression models with diagnostic plots
- Comprehensive PDF report (analysis_results.pdf)

## Author

Business Analytics Assignment - CSE5014
