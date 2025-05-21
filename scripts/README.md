# Streamlit Dashboard Development

## Overview
This directory contains scripts and documentation for the Streamlit dashboard developed for the Kifiya AI Mastery Bootcamp. The dashboard visualizes solar radiation data (GHI) across Benin, Sierra Leone, and Togo, allowing users to compare countries interactively.

## Folder Structure
- `app/`: Contains the Streamlit application.
  - `main.py`: Main app script with interactive widgets, GHI boxplot, and top regions table.
  - `utils.py`: Utility functions for data loading and visualization.
- `scripts/`: Contains this README and other potential scripts.
- `data/`: Stores cleaned CSVs (ignored in `.gitignore`).

## Development Process
1. **Branch**: Created `dashboard-dev` branch (`git checkout -b dashboard-dev`).
2. **Setup**: Added `app/` and `scripts/` folders with empty `__init__.py` files.
3. **App Development**:
   - `utils.py`: Functions to load CSVs, compute top regions, and plot boxplots.
   - `main.py`: Streamlit app with a multiselect widget for country selection, GHI boxplot, and top regions table.
4. **Git Hygiene**: Ensured `data/` is ignored in `.gitignore`. Committed changes with message: `feat: basic Streamlit UI`.
5. **Deployment**: Deployed to Streamlit Community Cloud (see below).

## Usage Instructions
1. **Prerequisites**:
   - Install dependencies: `pip install streamlit pandas seaborn matplotlib`
   - Ensure `data/benin_clean.csv`, `data/sierraleone_clean.csv`, and `data/togo_clean.csv` are in the `data/` folder.
2. **Run Locally**:
   ```bash
   streamlit run app/main.py

