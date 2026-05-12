# 🏀 NBA Salary Analysis: Who’s Overpaid and Underpaid in 2025?

A machine learning investigation into NBA market inefficiencies, using a **Random Forest Regression** model to predict player valuations based on 25 years of on-court performance data.

---

## 📝 Project Overview
This study examines the discrepancy between actual NBA salaries and "performance-justified" salaries for the 2025 season. By analyzing a dataset of **230,000+ records (2000–2025)**, the model identifies players whose contracts significantly deviate from their statistical output.

### 🎯 Key Performance Metrics
* **Model Accuracy:** R² = 0.75 | RMSE = $6,233,320
* **Primary Salary Drivers:** Points (PTS), Player Age, and Year (Salary Cap Inflation).
* **Underpaid Gem:** Spencer Dinwiddie (-87.4% relative to predicted value).
* **Overpaid Outlier:** Marvin Bagley III (+513.0% relative to predicted value).

---

## 🧪 Methodology & Formulas
The model predicts a "Fair Market Value" for each player based on a wide range of features including **PTS, MP, FG, DRB, AST, TOV,** and **GS**.

**Discrepancy Calculation:**
$$\text{Difference} = \text{Actual Salary} - \text{Predicted Salary}$$

**Percent Valuation:**
$$\text{Percent Over/Underpaid} = \left( \frac{\text{Difference}}{\text{Predicted Salary}} \right) \times 100$$

---

## 🛠 Tech Stack
- **Language:** Python
- **Modeling:** Scikit-Learn (Random Forest Regressor)
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Documentation:** [Policy Brief (PDF)](./Abdullahi_Cali_Policy_Brief.pdf)

---

## 📊 Key Findings
* **Position Bias:** Power Forwards (61.8%) and Small Forwards (61.0%) are the most frequently overpaid positions.
* **Market Opportunity:** Shooting Guards are the most undervalued group, with 54.7% earning less than their predicted performance value.
* **Veteran Value:** The model identified that age is a major predictor, suggesting teams often pay a premium for experience and "legacy" beyond raw box-score stats.

---

## 📂 Repository Structure
```text
NBA-Salary-Predictive-Model/
├── Abdullahi_Cali_Notebook.ipynb    # Data cleaning, EDA, and Model Training
├── Abdullahi_Cali_Policy_Brief.pdf  # Full summary and strategic recommendations
├── NBA_Player_Stats_2000-2025.csv   # Kaggle-sourced performance dataset
└── README.md                        # Project documentation
