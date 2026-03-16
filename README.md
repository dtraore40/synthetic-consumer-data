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


## Data

The `data/` directory is **ignored in this repository** to protect
sensitive or large datasets.

## Environment Setup

### 1️⃣ Python environment

To ensure reproducibility, the required Python packages are listed in
`requirements.txt`.

**Recreate the Python environment:**

```{Bash}
# Install all required packages
pip install -r requirements.txt
```

> Only the Python packages actually used in the project will be
> installed.

### 2️⃣ R environment

All R package dependencies are tracked using `renv`.

**Recreate the R environment:**

```{r}
# Install renv if not already installed
install.packages("renv")

# Restore R environment on another machine using renv.lock
renv::restore()
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
