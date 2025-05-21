# ☀️ Solar Data Discovery: Cross-Country Solar Farm Analysis

## 📌 Project Overview

This project is part of the 10 Academy's Week 0 challenge. The goal is to analyze solar radiation and environmental sensor data from **Benin**, **Togo**, and **Sierra Leone**. The aim is to identify the best regions for solar energy investments based on irradiance, temperature, humidity, and wind patterns.

The challenge is structured to simulate the responsibilities of a data or machine learning engineer working with real-world, messy datasets under time constraints.


## 📁 Repository Structure

```

solar-challenge-week1/
│
├── .github/workflows/       # GitHub Actions CI workflows
├── notebooks/               # Jupyter/Colab notebooks (EDA and comparison)
│   ├── benin\_eda.ipynb
│   ├── togo\_eda.ipynb
│   ├── sierra\_leone\_eda.ipynb
│   └── compare\_countries.ipynb
├── scripts/                 # Any data processing or utility scripts
├── tests/                   # Placeholder for unit tests
├── requirements.txt         # Python dependencies
├── README.md                # This file
├── .gitignore               # Files and folders to ignore in Git
└── data/                    # Cleaned data (ignored from Git)

````


## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/michaWorku/solar-challenge-week1.git
cd solar-challenge-week1
````

### 2. Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate     # or `venv\Scripts\activate` on Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Notebooks

Open Jupyter or Colab and explore the notebooks under the `notebooks/` directory.


## 🔍 Tasks Summary

### ✅ Task 1: Git & Environment Setup

* Created and configured repository with `.gitignore`, CI workflow, `requirements.txt`
* Set up GitHub Actions to test environment installation
* Used pull request and branching workflow

### ✅ Task 2: Data Cleaning & EDA

* Cleaned and profiled solar datasets for each country
* Conducted:

  * Missing value analysis
  * Outlier detection (Z-scores)
  * Time series analysis
  * Cleaning impact analysis
  * Correlation heatmaps and scatterplots
  * Wind and temperature distribution analysis
  * Bubble charts to visualize RH vs temperature and irradiance

### ✅ Task 3: Cross-Country Comparison

* Combined all cleaned datasets into one
* Created comparative boxplots and summary tables (mean, median, std)
* Performed statistical testing (ANOVA and Kruskal–Wallis)
* Summarized findings with visual and textual insights


## 📊 Key Observations

* **Benin** shows the highest average and median GHI, making it the most promising candidate for solar investment.
* **Togo** demonstrates higher variability in GHI, suggesting less predictable solar potential.
* **Sierraleone** has consistently lower GHI, but more stable readings, which may still be viable depending on cost and infrastructure.


## 📑 References

* [10 Academy Challenge Guide (PDF)](https://docs.google.com/document/d/1HsCSC_RZk_sj39Cc30OwFX9DLvUoh2OW7Eq0y1Dsf8E/edit?tab=t.0#heading=h.owazencuc4hr)
* [Solar Radiation Measurement Dataset](https://energydata.info/dataset/?q=Solar+Radiation+Measurement&vocab_regions=AFR)
* [Seaborn Documentation](https://seaborn.pydata.org/)
* [scipy.stats documentation (ANOVA, Kruskal)](https://docs.scipy.org/doc/scipy/)


## 📃 License

This project is for educational purposes as part of the 10 Academy training program.
