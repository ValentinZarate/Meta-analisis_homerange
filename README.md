# Meta-analysis of Production Landscapes Effects on Mammal Home Range Size

This repository contains the data extraction, harmonization, and analysis workflow for a meta-analysis evaluating the effects of human production systems (agriculture and forestry) on mammalian home range size.

The analysis focuses on comparing home range estimates between natural and production landscapes using standardized effect sizes (Cohen’s *d*).

### Literature search was conducted using constumized workflow and R functions, more details in [Search Cycle](https://github.com/ValentinZarate/bib_functions/blob/main/Search%20Cylce/cylce.md)
---

## Study Scope

- Taxa: Mammals  
- Land-use types:
  - Natural / low-disturbance habitats
  - Agricultural systems
  - Forestry systems
- Response variable: Home range size
- Effect size metric: Cohen’s *d*

---

## Data Extraction and Harmonization

For each study included in the meta-analysis, the following information was extracted when available:

- Mean home range size
- Standard deviation (SD) or variance
- Sample size
- Species
- Study system and location
- Land-use category (natural vs production)

When necessary, reported metrics were transformed to ensure comparability across studies (e.g. unit standardization, SD derivation from confidence intervals or standard errors).

---

## Analysis Workflow

The main steps of the analysis include:

1. Extraction and standardization of mean and SD values  
2. Calculation of effect sizes (Cohen’s *d*)  
3. Comparison of effect sizes across land-use types  
4. Sensitivity analyses and exploration of heterogeneity  

Analyses were conducted in R following standard meta-analytic procedures.

---

## Repository Structure
```
Meta-analisis_homerange/
│
├── data/ # Extracted and harmonized data
├── scripts/ # R scripts for effect size calculation and analysis
├── output/ # Tables, figures, and model outputs
├── comparaciones_dia por dia.md
│ # Step-by-step comparison notes and decisions
└── README.md
```
