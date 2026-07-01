# 🐸 GBIF Brazilian Amphibian Biodiversity Analysis

This project presents an exploratory and statistical analysis of amphibian occurrence records in Brazil using data from the Global Biodiversity Information Facility (GBIF).

The workflow combines data engineering, spatial filtering, exploratory data analysis, and statistical modeling to investigate large-scale patterns in biodiversity data and associated sampling biases.

---

## 📊 Objectives

The main goals of this project are:

- Clean and structure GBIF occurrence data
- Assess spatial, temporal, and taxonomic sampling biases
- Evaluate species richness patterns across Brazil
- Model temporal trends in data collection using statistical approaches
- Visualize biodiversity patterns using interactive maps and ecological methods

---

## 🧰 Workflow Overview

### 1. Data Engineering (SQL ETL)
- Filtering raw GBIF occurrence data
- Removing inconsistent and low-quality records
- Standardizing taxonomic and geographic fields
- Creating a cleaned analytical dataset

### 2. Spatial Quality Control
- Detection and removal of coordinate outliers
- Classification of spatially valid records
- Visualization of geographic distribution of occurrences

### 3. Exploratory Data Analysis
- Temporal distribution of records (decades)
- Institutional contribution patterns
- State-level richness and sampling intensity

### 4. Sampling Bias Analysis
- Spatial sampling bias
- Taxonomic dominance patterns
- Species-level accumulation distributions

### 5. Statistical Modeling
- Poisson GLM for temporal trends in occurrence records
- Evaluation of long-term data collection dynamics

### 6. Ecological Modeling
- Species accumulation curves
- Rarefaction analysis with permutation-based smoothing

### 7. Geospatial Visualization
- Interactive maps using Plotly
- Spatial-temporal distribution of records
- Density-based visualization of sampling effort

---

## 📈 Key Insights

- Strong **spatial bias** toward southeastern and northern Brazil
- Significant **temporal increase** in records, especially after 1950 and 2000
- High **taxonomic unevenness**, with a small subset of species dominating records
- Evidence of **incomplete sampling saturation** at national scale
- Data structure strongly influenced by **historical and institutional sampling effort**

---

## ⚠️ Data Limitations

This dataset reflects occurrence records from GBIF and is subject to:

- Uneven spatial sampling effort
- Historical bias in museum collections
- Taxonomic overrepresentation of well-studied groups
- Temporal bias due to digitization processes
- Gaps in remote and under-sampled regions

All analyses should be interpreted considering these limitations.

---

## 🛠️ Tools & Technologies

- Python (Pandas, NumPy, Matplotlib, Plotly)
- Statsmodels (GLM - Poisson regression)
- SQL (ETL pipeline)
- Geospatial analysis (coordinate filtering & mapping)
- Jupyter Notebook

---

## 📂 Data Sources

- Global Biodiversity Information Facility (GBIF)
- Processed occurrence dataset of Brazilian amphibians

---

## 📌 Author

Felipe Andrade  
Biodiversity, Systematics & Data Science

---

## 🚀 Future Work

- Species distribution modeling (SDM)
- Spatial autocorrelation analysis
- Bayesian hierarchical models for sampling bias
- Integration with environmental predictors (climate, land cover)

---
