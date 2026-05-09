# Data (Nigeria climate + food security)

This folder contains datasets curated for exploratory analysis supporting the review paper:
**“The Impact of Climate Change on Food Security in Nigeria: A Review of Empirical and Theoretical Evidence.”**

## Folder structure
- `data/raw/` — downloaded/raw files (do not edit manually)
- `data/processed/` — cleaned/merged analysis-ready datasets created by the notebook

## Sources curated in the notebook

### 1) NASA POWER (climate)
- Variables (monthly): precipitation and near-surface air temperature.
- Coverage: long-run historical monthly series (depends on NASA POWER availability).
- Geography: Nigeria approximated by a single lat/lon point (country centroid).
- Purpose: simple national-level climate signal for benchmarking relationships.

### 2) World Bank World Development Indicators (food security & agriculture proxies)
Examples of indicators the notebook attempts to download (availability varies by year):
- Cereal yield (kg per hectare)
- Food production index
- Agriculture value added (% of GDP)
- Prevalence of undernourishment / food insecurity indicators (where available)

Notes:
- These are proxies at national scale and are not substitutes for household survey microdata.
- The notebook logs which indicators were successfully downloaded.

## Reproducibility
Run the notebook `World_ai.ipynb` from top to bottom. It will:
1. Download raw datasets into `data/raw/`
2. Create cleaned/merged outputs in `data/processed/`
3. Produce basic EDA summaries and plots
