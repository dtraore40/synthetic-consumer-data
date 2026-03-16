---
title: "project_structure"
format: html
---

## Project Structure

```{r}
synthetic-consumer-data/
│
├── data/                    # Data folder (ignored on GitHub)
│   ├── raw/                 # Original datasets (no modifications)
│   └── processed/           # Cleaned / transformed datasets
│
├── scripts/                 # Scripts for data generation and preprocessing
│   ├── data_generation.R
│   └── preprocessing.py
│
├── notebooks/               # Exploratory analysis and experiments
│
├── results/                 # Outputs, figures, and model results
│
├── docs/
│   ├── project_structure.md 
│   ├── data_dictionary.qmd  
│   └── reproducibility.qmd  
│
├── renv/                    # Internal R environment folder (ignored by Git)
├── renv.lock                # R package dependencies for reproducibility
├──.Rprofile                 # Automatically activates renv
│
├── requirements.txt         # Python dependencies for reproducibility
│
├── .gitignore               # Git ignore rules
└── README.md                # Project documentation

```