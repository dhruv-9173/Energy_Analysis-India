# Energy Analysis — India

**Course:** CA-2 INT375 Data Science ToolBox: Python Programming  
**Repository:** `dhruv-9173/Energy_Analysis-India`  
**Last updated:** 2026-04-26

---

## Table of Contents
- [Overview](#overview)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Environment & Setup](#environment--setup)
  - [Option A: Run locally (recommended)](#option-a-run-locally-recommended)
- [How to Run](#how-to-run)
- [Methodology](#methodology)
- [Visualizations](#visualizations)
- [Results & Insights](#results--insights)
- [Tech Stack](#tech-stack)
- [Contributing](#contributing)
- [Acknowledgements](#acknowledgements)

---

## Overview
This project analyzes **energy-related data for India** using Python. It focuses on cleaning, exploring, and visualizing the dataset to identify patterns, trends, and insights that support data-driven interpretation.

This repository was created as part of the **CA-2 assessment** for **INT375 (Data Science ToolBox: Python Programming)**.

---

## Objectives
- Load and validate the dataset (types, missing values, duplicates).
- Perform exploratory data analysis (EDA) to understand distributions and trends.
- Create meaningful visualizations to communicate findings clearly.
- Summarize key insights and observations from the analysis.

---

## Dataset
Describe your dataset clearly here.

**Dataset name:** *Potential, Generation, Capacity - Renewable*  
**Source:** *https://ndap.niti.gov.in/*  
**Time period covered:** *2006-2020*  
**Geography:** *36 Indian States and Union Territories*  
**Granularity:** *Yearly*

## Environment & Setup

### Option A: Run locally (recommended)
1. **Clone the repository**
   ```bash
   git clone https://github.com/dhruv-9173/Energy_Analysis-India.git
   cd Energy_Analysis-India
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv .venv
   # Windows (PowerShell)
   .\.venv\Scripts\Activate.ps1
   # macOS/Linux
   source .venv/bin/activate
   ```

3. **Install dependencies**
   - If you have `requirements.txt`:
     ```bash
     pip install -r requirements.txt
     ```
   - Otherwise, install core packages commonly used for EDA:
     ```bash
     pip install numpy pandas matplotlib seaborn plotly jupyter
     ```

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

---

## How to Run
> Adjust notebook/script names to match your repo.

### Run the notebook
- Open `notebooks/<your_notebook_name>.ipynb`
- Run cells top-to-bottom

### Run via script (optional)
If you have a script-based workflow:
```bash
python src/main.py
```

---

## Methodology
This project follows a standard data analysis pipeline:

1. **Data Ingestion**
   - Import data from CSV/Excel/other formats.
   - Check schema, data types, and basic validity.

2. **Data Cleaning**
   - Handle missing values
   - Remove duplicates (if applicable)
   - Convert units / standardize categories
   - Parse dates/years correctly

3. **Exploratory Data Analysis (EDA)**
   - Descriptive statistics (mean/median/std)
   - Group-by analysis (by year/state/sector, etc.)
   - Outlier checks and distribution exploration

4. **Visualization & Interpretation**
   - Trend plots, comparisons, and breakdowns
   - Insights captured as bullet points and summary statements

---

## Visualizations

### Visualization 1 — *Renewable Vs Non-Renewable Energy Generation(2006-2020)*

<img width="715" height="239" alt="image" src="https://github.com/user-attachments/assets/d80363bb-cfea-4f9f-b280-3d360c5ab744" />

---

### Visualization 2 — *Top 10 States - Energy Analysis*

<img width="715" height="195" alt="image" src="https://github.com/user-attachments/assets/002ab4f6-b125-4c61-b0c6-4fe9a30e2c33" />

---

### Visualization 3 — *Total Generation Enrergy Source*

<img width="712" height="262" alt="image" src="https://github.com/user-attachments/assets/2465ca8b-1862-495b-9d43-5b95234613e7" />

---

### Visualization 4 — *Time-Series Analysis Energy Generation*

<img width="711" height="343" alt="image" src="https://github.com/user-attachments/assets/a8c26cf5-09ee-4086-9752-878396cab44e" />

---

### Visualization 5 — *Outlier Detection - Value MW By Category*

<img width="712" height="236" alt="image" src="https://github.com/user-attachments/assets/2d3b27de-7779-4c02-a397-ffaa429a3a4b" />

---

## Results & Insights
<img width="712" height="332" alt="image" src="https://github.com/user-attachments/assets/15bb0aaf-f4ce-46db-b979-f397342d8b7e" />
<img width="712" height="315" alt="image" src="https://github.com/user-attachments/assets/a8cd3442-cd3c-4d22-9cb1-8b3817ab7c7c" />


The correlation matrix revealed that Year has a moderate positive correlation with Value_MW, confirming the temporal growth trend in energy generation. The Nature column (encoded) showed a negative correlation with Value_MW for non-renewable sources, consistent with the dominance of renewable in smaller installations. Most categorical variables showed weak correlations with each other, confirming the independence of the engineered features.

The renewable generation heatmap revealed that states such as Maharashtra, Tamil Nadu, Karnataka, and Rajasthan showed the most consistent and darkest shading across all years — indicating sustained high renewable generation throughout the study period. States in the northeast showed lighter shading, reflecting lower installed capacity. A clear intensification of colour was observed from 2012 onwards across most states, corresponding to the national acceleration in renewable capacity addition.

---

## Tech Stack
- **Language:** Python
- **Core libraries:** NumPy, Pandas
- **Visualization:** Matplotlib, Seaborn 
- **Environment:** Jupyter Notebook / JupyterLab

---

## Contributing
This repository is primarily for coursework submission, but improvements are welcome.

To contribute:
1. Fork the repo
2. Create a feature branch: `git checkout -b feature/<name>`
3. Commit changes
4. Open a Pull Request

---


## Acknowledgements
- Course: **INT375 Data Science ToolBox: Python Programming**
- Instructor/Institution: *Dr. Savleen Kaur*

# ADD TREND FORECASTING CHART
