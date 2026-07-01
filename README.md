# 🐸 GBIF Amphibian Data Analysis (Python EDA)

## Overview

This project presents an exploratory and statistical analysis of amphibian occurrence records in Brazil using a cleaned dataset derived from GBIF.

The goal is to move beyond data engineering and focus on **data interpretation**, exploring spatial, temporal, and taxonomic patterns using Python-based analytical workflows.

This repository represents the **analytical phase** of a broader biodiversity data pipeline.

---

## 🧠 Analytical Focus

Unlike the previous SQL-based ETL pipeline, this project focuses on:

- Exploratory Data Analysis (EDA)
- Spatial and temporal pattern detection
- Statistical modeling of biodiversity records
- Sampling and taxonomic bias assessment
- Ecological interpretation of large-scale occurrence data

---

## 📊 Dataset

The dataset used in this analysis is the cleaned output from the GBIF ETL pipeline.

- **Records:** 399,333 occurrence records
- **Filtered valid spatial records:** subset used for spatial analyses
- **Temporal coverage:** 1830–2020+
- **Geographic scope:** Brazil (with standardized state-level classification)

> ⚠️ Raw GBIF data is not included due to size constraints.  
> This analysis uses the processed dataset generated in the ETL pipeline.

---

## 📓 Main Notebook

All analyses are contained in:

- `01_exploratory_analysis.ipynb`

This notebook includes:

### 1. Data Quality Assessment
- Missing data profiling
- Completeness analysis
- Spatial filtering of coordinate outliers

### 2. Temporal Analysis
- Occurrence trends across decades
- Temporal distribution of records
- GLM (Poisson regression) for temporal trend modeling

### 3. Spatial Analysis
- Geographic distribution of records
- State-level richness and sampling intensity
- Spatial bias detection

### 4. Sampling Bias Analysis
- Institutional bias
- Geographic sampling imbalance
- Species-level representation patterns

### 5. Taxonomic Structure
- Family, genus, and species dominance
- Rank-abundance patterns
- Identification of highly skewed distributions

### 6. Ecological Modeling
- Species accumulation curves
- Rarefaction analysis (permutation-based)

### 7. Geospatial Visualization
- Interactive maps using Plotly
- Spatial-temporal visualization of occurrence records

---

## 📈 Key Insights

- Strong **spatial sampling bias**, with concentration in southeastern and northern Brazil
- Highly **uneven institutional contribution**, with a few institutions dominating records
- Strong **temporal exponential growth** in occurrence data, confirmed by GLM
- Significant **taxonomic imbalance**, with a small subset of species dominating observations
- Evidence of **incomplete sampling saturation** across Brazilian amphibian diversity
- Clear interaction between **historical sampling effort and data availability**

---

## ⚠️ Analytical Considerations

All results should be interpreted in the context of:

- Non-random sampling processes
- Historical accumulation of museum records
- Digitization-driven temporal bias
- Geographic accessibility constraints
- Taxonomic research bias toward certain groups

This dataset reflects **sampling effort structure**, not direct ecological abundance.

---

## 🧰 Tools & Technologies

- Python (Pandas, NumPy)
- Matplotlib / Plotly
- Statsmodels (GLM – Poisson regression)
- SciPy (statistical analysis)
- Jupyter Notebook

---

## 📁 Repository Structure

```
├── 01_exploratory_analysis.ipynb   # Main analysis notebook
├── requirements.txt                # Python dependencies
└── README.md
```

---

## 🔁 Reproducibility

To reproduce this analysis:

```bash
git clone https://github.com/your-username/gbif-amphibian-python-analysis.git
cd gbif-amphibian-python-analysis

pip install -r requirements.txt

jupyter notebook
```

---

## 🚀 Future Work

- Species distribution modeling (SDM)
- Spatial autocorrelation analysis
- Bayesian modeling of sampling bias
- Integration with environmental predictors
- Interactive dashboard (Streamlit / Plotly Dash)

---

## 👤 Author

Felipe Andrade  

---
