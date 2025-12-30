# 🌍 Global COVID-19 Data Analysis: Uncovering Hidden Patterns & Causality

![Python](https://img.shields.io/badge/Python-3.9-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-ffffff?style=for-the-badge&logo=matplotlib)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 📖 Overview

This project is not just another COVID-19 dashboard. It is an advanced data analysis study that aims to debunk common statistical misconceptions and uncover the **root causes** behind mortality rates using the **"Our World in Data"** dataset.

As an Industrial Engineering student, I approached this problem with a systems thinking mindset—focusing on variable isolation, lag effects, and capacity planning (healthcare infrastructure).

**📄 [Read the Full Report (PDF)](./covid_report.pdf)**
**📊 [View the Presentation (PDF)](./Global-COVID-19-Data-Analysis.pdf)**

---

## 🔍 Key Findings & methodology

### 1. Debunking Simpson's Paradox (Demographics vs. Habits)
Initial data showed a misleading negative correlation (-0.07) between smoking and death rates. By stratifying the data, I revealed that **Age** was the confounding variable.
* **Result:** Correcting for age revealed a strong positive correlation (+0.65) between median age/smoking and mortality.

### 2. The "Cumulative Trap" in Vaccination Efficacy
Cumulative plots failed to show the immediate impact of vaccines due to historical death tolls.
* **Method:** I used a **Binning Approach** (0-10% to >70% vaccination milestones) to analyze *Daily Deaths per Million*.
* **Result:** A step-down trend was proven; daily deaths dropped significantly as countries passed the 50% vaccination threshold.

### 3. The Healthcare Infrastructure Paradox
Analysis showed that having high hospital bed capacity did not guarantee lower mortality in developed nations (e.g., Eastern Europe).
* **Root Cause:** Using a multi-variable scatter plot, I identified **Cardiovascular Death Rate** as the hidden driver. High comorbidity rates in a population outweigh the logistical benefits of hospital beds.

### 4. Policy Analysis: The "Reactive Cycle"
A dual-axis time-series analysis of the **Stringency Index** vs. **New Cases** for key countries (e.g., Germany, Turkey).
* **Insight:** Government restrictions consistently exhibited a "Lag Effect," spiking *after* infection waves began, indicating a **reactive** rather than proactive policy-making approach.

---

## 🛠️ Tech Stack

* **Language:** Python 3.9
* **Libraries:**
    * `Pandas` (Data Cleaning, Grouping, Time-series manipulation)
    * `Matplotlib` & `Seaborn` (Statistical Visualization)
    * `NumPy` (Numerical operations)
* **Tools:** Jupyter Notebook, MS Excel (Data Source), Gamma (Presentation).

---

## 🚀 How to Run the Analysis

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YusufArslan-ie/covid-data-analysis.git](https://github.com/YusufArslan-ie/covid-data-analysis.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas matplotlib seaborn numpy openpyxl
    ```
3.  **Run the Notebook:**
    Open `jupyter.ipynb` and `jupyter2.ipynb` in Jupyter Notebook or VS Code to reproduce the charts.

---

## ✍️ Author

**Yusuf Mehmet Arslan**
* Industrial Engineering Student
* Passionate about Data Science, Process Optimization, and Business Intelligence.

[LinkedIn Profile](https://www.linkedin.com/in/yusuf-arslan-948160216/) | [Email Me](yusufarslan.ie@gmail.com)
