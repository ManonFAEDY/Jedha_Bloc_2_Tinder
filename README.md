# 💖 Tinder Speed Dating Interest Analysis

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Pandas](https://img.shields.io/badge/Pandas-v1.4+-red.svg)](https://pandas.pydata.org/)
[![Matplotlib/Seaborn](https://img.shields.io/badge/Viz-Matplotlib%2FSeaborn-blueviolet.svg)](https://seaborn.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Exploratory Data Analysis (EDA) project to uncover the key factors influencing mutual interest and the decision to go on a second date, using data from a speed dating experiment.**

---

## 📋 Table of Contents
- [Context](#-context)
- [Project Objective](#-project-objective)
- [Data & Scope](#-data--scope)
- [Technologies](#-technologies)
- [Deliverables](#-deliverables)
- [Methodology](#-methodology)
- [Data Exploration Ideas](#-data-exploration-ideas)
- [Installation & Execution](#-installation--execution)
- [Author](#-author)

---

## 🎯 Context

**Tinder**, a global leader in online dating, is seeking to understand the dynamics of **initial attraction and mutual interest** following a decrease in match rates. To address this, the marketing team conducted a **speed dating experiment**, gathering detailed behavioral and self-perception data.

**Mission:** Analyze the rich dataset from this experiment to identify the variables (attributes, demographics, preferences) that best predict the decision to agree to a **second date**.

---

## 🚀 Project Objective

This project aims to provide the marketing team with a **clear, data-backed understanding** of attraction to inform potential feature development or marketing strategies. The analysis is divided into two main steps:

### 1. **Data Cleaning & Preparation**
- Handle the complex, multi-source dataset (individual and paired-date level).
- Clean and organize variables including demographics, self-perceptions, and in-date ratings.
- Manage missing values and prepare features for descriptive analysis.

### 2. **Descriptive Statistics & Visualization**
- Calculate key **descriptive statistics** (means, distributions, counts) on critical attributes.
- Create impactful **visualizations** (histograms, bar plots, box plots) to highlight correlations with the **second date decision**.
- Provide clear **captions and interpretations** for all findings, directly addressing the core question of mutual interest.

---

## 📊 Data & Scope

### Source
Data was gathered from an experimental series of **speed dating events** held between 2002-2004.

### Key Dataset Features
Each row represents a **single 4-minute speed date**. The dataset includes:

| Category | Columns (Examples) | Role |
| :--- | :--- | :--- |
| **Target (Y)** | `dec`, `dec_o` (Decision of each partner) | Binary variables indicating agreement to a second date. |
| **In-Date Ratings** | `attr`, `sinc`, `intel`, `fun`, `amb`, `shar` | Ratings given to the date on 6 key attributes. |
| **Self-Perception** | `s_attr`, `s_sinc`, `s_intel`, etc. | Participants' self-assessment on the 6 attributes. |
| **Demographics** | `gender`, `age`, `race`, `field` | Personal and background information. |

### Project Scope
Analysis is focused on finding predictors of the **second date agreement**, utilizing demographics, self-perception, stated preferences, and in-date ratings.

---

## 🛠️ Technologies

The project will be developed using a **Python** environment, prioritizing standard data science libraries for analysis and visualization.

### Languages & Libraries
```python
pandas              # Data cleaning and preparation
numpy                # Numerical computing
matplotlib/seaborn   # Visualizations and statistical plotting
````

-----

## 📁 Project Structure

```
tinder-interest-analysis/
│
├── 📓 Project_Tinder.ipynb                        # Main notebook for all analysis
├── 📝 README.md                                # This file
└── 🖼️ img/                                    # Folder for exported charts and graphs
```

-----

## 🔬 Methodology

### Part 1: Data Preparation

1.  **Data Loading & Merging:** Load the main dataset and potentially merge with attribute keys for clarity.
2.  **Creating the Target Variable:** Focus on the 'decision' variables (`dec`, `dec_o`) and potentially derive a **`Match`** variable (where both parties said 'yes').
3.  **Feature Cleaning:** Standardize scales, handle categorical variables (e.g., race, field of study), and address ratings data.

### Part 2: Exploratory Data Analysis (EDA)

1.  What attributes do people look for in the opposite sex?
2.  Are shared interests more important than a shared racial background?
3.  How people who get matchs & go on dates are rated by others?
4.  In terms of getting a second date, is it better to be someone's first speed date of the night or their last?
5.  Can people accurately predict their own perceived value in the dating market?
6.  Which attributes are most correlated with matchs?

-----

## 💻 Installation & Execution

To replicate this analysis, you'll need a standard Python environment.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/votre_profil/votre_repo.git](https://github.com/votre_profil/votre_repo.git)
    cd tinder-interest-analysis
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  **Open and Execute the Notebook:**
    Launch the `tinder_speed_dating_analysis.ipynb` notebook and run the cells sequentially.
    ```bash
    jupyter notebook tinder_speed_dating_analysis.ipynb
    ```

-----

## 👤 Author

**[Manon FAEDY]**

  * 🐙 [GitHub](https://www.google.com/search?q=https://github.com/ManonFAEDY)

-----

## 📄 License

This project is licensed under the MIT License.

-----

## 🙏 Acknowledgments

  * **Tinder** for the project initiative.
  * **Columbia Business School** for making the Speed Dating data publicly available for research.
  * **Jedha** for the project framework.

-----

⭐ A data-driven insight on love and attraction\! Star the repo if you found the analysis insightful\! ⭐
