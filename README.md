# Synthetic Consumer Data

Synthetic data generation and modeling for consumer behavior analysis.

## Project Overview

This project explores methods for **generating synthetic consumer**
**datasets** and analyzing consumer behavior while preserving privacy.
Synthetic data can help simulate realistic consumer patterns and support
**market research, modeling, and experimentation** when real data is
limited or confidential.

The project combines **R and Python** for data generation,
preprocessing, and exploratory analysis.

## Technologies

-   **Python**
-   **R**
-   **RStudio**
-   **Pandas**, **NumPy**, **Scikit-learn**
-   **Jupyter Notebooks**
-   **R Markdown**

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
├── renv/                    # Internal R environment folder (ignored by Git)
├── renv.lock                # R package dependencies for reproducibility
├── requirements.txt         # Python dependencies for reproducibility
├── .gitignore               # Git ignore rules
└── README.md                # Project documentation

```

## Data

The `data/` directory is **ignored in this repository** to protect
sensitive or large datasets.

## Environment Setup

### 1️⃣ Python environment

To ensure reproducibility, the required Python packages are listed in
`requirements.txt`.

**Steps to recreate the Python environment:**

```{Bash}
# Install pipreqs (optional, for regenerating requirements.txt)
pip install pipreqs

# Install all required packages
pip install -r requirements.txt

# Generate or update requirements.txt based on the packages actually used
pipreqs ./ --force
```

> Only the Python packages actually used in the project will be
> installed.

### 2️⃣ R environment

All R package dependencies are tracked using `renv`.

**Steps to recreate the R environment:**

```{r}
# Install renv if not already installed
install.packages("renv")

# Restore R environment on another machine using renv.lock
renv::restore()

# Initialize renv for a new R project (optional if the project is already set up)
renv::init()

# Save current R packages to renv.lock after installing new packages
renv::snapshot()
```

> `renv.lock` ensures that **all required R packages with the exact
> versions** are installed, reproducing the original environment for the
> project.

## Notes

-   Restore the **R environment first** before running any R scripts.
-   Install **Python packages** before running Python scripts.
-   This guarantees that all scripts and notebooks run **without**
    **dependency issues.**

## Objectives

-   Generate **synthetic consumer datasets**
-   Simulate **consumer behavior patterns**
-   Perform **data preprocessing and feature engineering**
-   Explore insights using **data analysis and modeling**

## Future Work

-   Implement advanced **synthetic data generation techniques**
-   Evaluate **data quality and realism**
