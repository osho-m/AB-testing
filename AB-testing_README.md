# A/B Test Analysis on Marketing Data

A statistical analysis project that evaluates the effectiveness of a **marketing ad campaign** using A/B testing on real-world marketing data. The project determines whether ads drove statistically significant conversions compared to a control group shown a Public Service Announcement (PSA).

---

## 📌 Project Overview

Marketing companies run A/B tests to compare two versions of a campaign on different user segments simultaneously. This project answers two core business questions:

1. **Was the ad campaign successful?**
2. **How much of the conversion success can be attributed to the ads?**

---

## 📊 Dataset

**File:** `marketing_AB.csv`  
**Size:** 588,101 users

| Feature | Description |
|---|---|
| `user id` | Unique user identifier |
| `test group` | `ad` — saw the advertisement; `psa` — saw the Public Service Announcement |
| `converted` | `True` if user purchased the product; `False` otherwise |
| `total ads` | Total number of ads seen by the user |
| `most ads day` | Day of the week the user saw the most ads |
| `most ads hour` | Hour of the day the user saw the most ads |

### Key Dataset Stats
- **Total users:** 588,101
- **Ad group:** 564,577 users
- **PSA group:** 23,524 users
- **Average ads seen per user:** ~24.8
- **Most common day for ad exposure:** Friday

---

## 🔬 Analysis Workflow

1. **Data Loading & Cleaning** — Load dataset, drop unnecessary index column
2. **Exploratory Data Analysis (EDA)** — Descriptive statistics, group distributions
3. **Conversion Rate Analysis** — Compare conversion rates between `ad` and `psa` groups
4. **Visualisation** — Bar plots, conversion breakdowns by day and hour using Seaborn, Matplotlib, and Plotly
5. **Statistical Significance Testing** — Chi-square / proportion z-test to validate results

---

## 🛠️ Tech Stack

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly Express
- SciPy

---

## 📁 Project Structure

```
AB-testing/
│
└── code/
    └── A_B_test_analysis_on_marketing_data.ipynb   # Full analysis notebook
```

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn plotly scipy
```

### Run the Notebook

```bash
jupyter notebook code/A_B_test_analysis_on_marketing_data.ipynb
```

> **Note:** Place `marketing_AB.csv` in the working directory before running.

---

## 🔍 Key Concepts Demonstrated

- **A/B Testing Framework** — Experimental vs control group design
- **Conversion Rate Analysis** — Measuring campaign effectiveness
- **Statistical Significance Testing** — Determining if results are not due to chance
- **Data Visualisation** — Identifying patterns by day, hour, and group
- **Business Insight Generation** — Translating statistical results into actionable conclusions

---

## 💡 Business Context

> *"The idea of the dataset is to analyze the groups, find if the ads were successful, how much the company can make from the ads, and if the difference between the groups is statistically significant."*

---

## 👤 Author

**Osho Muralidaran**  
[LinkedIn](https://www.linkedin.com/in/osho-m) · [GitHub](https://github.com/osho-m)
