# income-inequality-colombia

A comprehensive analysis of income inequality in Colombia using the 2024 GEIH dataset. This repository includes data processing, descriptive statistics, visualizations, and policy-oriented insights into socioeconomic disparities across regions and social classes.

---

## Overview

This project explores the distribution of household incomes in Colombia, identifies the main socioeconomic variables distinguishing high- and low-income households, and uncovers regional patterns of inequality. We leverage the GEIH (Gran Encuesta Integrada de Hogares) 2024 microdata to:

- Compute central-tendency and dispersion metrics  
- Visualize skewness, outliers, and class-based differences  
- Map geographic disparities  
- Assess labor, education, housing, and demographic factors  
- Formulate data-driven policy recommendations  

---

## Data Description
- **Source:** DANE’s GEIH microdata (2024)  
- **Coverage:** Non-institutional civilian households across all Colombian departments (except Providencia & San Andrés)  
- **Key Variables:**  
  - `Ingresos_finales`: Total monthly household income (COP)  
  - **Demographics:** household size, education level, number of children  
  - **Labor:** contract type, formal employment status, tenure, pension contributions  
  - **Housing:** ownership status, rental or mortgage payments  
  - **Geography:** department codes, region classifications


## File Structure

```plaintext
.
├── GEIH Analisis.do   # Main Python script with all the project and conclutions
├── DATA               # The necesary DataFrames to run the project local
└── README.md          # Project documentation
```

## Requirements
- **Python:** 3.8 or higher  
- **Environment:** Jupyter Notebook or JupyterLab  
- **Dependencies:**  
  - pandas  
  - numpy  
  - matplotlib  
  - seaborn  
  - scipy  
  - geopandas  
  - folium  

## Analysis Workflow
1. **Descriptive Statistics:** Compute mean, median, mode, SD, range, skewness, kurtosis; plot histograms and boxplots (linear & log scales).  
2. **Outlier Detection:** Identify extremes via IQR criterion and z-score thresholding.  
3. **Class Definitions:** Map DANE class proportions (60% low, 35% middle, 5% high) to household income ranges.  
4. **Socioeconomic Profiling:** Compare education, contract type, formalization, tenure, and job demands across classes.  
5. **Geographic Patterns:** Generate department-level heatmaps and regional choropleths for income and education.  
6. **Policy Insights:** Synthesize findings into targeted recommendations.  

## Key Findings
- **Highly right-skewed distribution:** Mean (2.38 M COP) ≫ median (1.30 M COP); 75% earn < 2.3 M COP.  
- **Housing burden:** Rent/mortgage consumes 30–37% of income for most households.  
- **Educational divide:** Upper class median at university level vs. basic secondary for low-income.  
- **Labor formalization gap:** 94% of upper class under formal contracts vs. 21–51% in low-income groups.  
- **Regional inequality:** Andean region leads in income; Pacific and Caribbean lag despite high education levels.  
- **Structural poverty:** Majority live below living‐wage thresholds, creating a persistent poverty cycle.  

## Policy Recommendations
1. **Invest in education:** Expand technical and tertiary programs to boost access to formal, higher-paying jobs.  
2. **Promote labor formalization:** Offer incentives and reforms for stable contracts and pension contributions, especially in lagging regions.  
3. **Support regional development:** Improve infrastructure to lower costs of housing, healthcare, and food.  
4. **Combat corruption & strengthen institutions:** Ensure equitable opportunities nationwide to break the cycle of structural poverty.  

