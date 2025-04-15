# Home.LLC - Assignment for Hiring

# 🏠 US Home Price Modeling (2005–2025)

This project explores how key macroeconomic factors have influenced U.S. home prices over the past 20 years using publicly available data. The **S&P CoreLogic Case-Shiller U.S. National Home Price Index** is used as the target variable to represent national-level home prices.

---

## 📌 Objective

To build a data science model that explains how key economic indicators such as mortgage rates, GDP, inflation, unemployment, and building permits have impacted home prices in the United States from 2005 to 2025.

---

## 📊 Data Sources

All data was collected from publicly available sources, primarily [FRED (Federal Reserve Economic Data)](https://fred.stlouisfed.org/):

| Feature            | Description                                           | FRED Series ID   |
|--------------------|-------------------------------------------------------|------------------|
| Home Price Index   | S&P/Case-Shiller U.S. National Home Price Index      | `CSUSHPISA`      |
| Mortgage Rate      | 30-Year Fixed Rate Mortgage Average in the US        | `MORTGAGE30US`   |
| Unemployment Rate  | Civilian Unemployment Rate                           | `UNRATE`         |
| GDP                | Gross Domestic Product                                | `GDP`            |
| Inflation          | Consumer Price Index (CPI-U)                          | `CPIAUCSL`       |
| Building Permits   | New Privately-Owned Housing Units Authorized          | `PERMIT`         |
| Population         | Total US Population                                   | `POP`            |

All datasets were collected, resampled to a quarterly frequency, cleaned, and merged for analysis.

---

## ⚙️ Tools & Libraries

- Python 3
- Jupyter Notebook
- pandas, numpy
- matplotlib, seaborn
- scikit-learn (for modeling)

---

## 🧠 Modeling Approach

Three models were used to understand the relationships and make predictions:

- **Linear Regression**: Baseline model for interpretability.
- **Random Forest Regressor**: Non-linear model capturing complex relationships.
- **Lasso Regression**: For feature selection and preventing overfitting.

---

## 📈 Results

| Model              | R² Score | RMSE   |
|-------------------|----------|--------|
| Linear Regression | 0.84     | 3.12   |
| Random Forest     | 0.89     | 2.48   |
| Lasso Regression  | 0.78     | 3.56   |

---

## 🔍 Key Insights

- **Mortgage Rates** show a strong inverse correlation with home prices.
- **GDP** growth positively influences housing demand and price increases.
- **Unemployment** and **CPI** (inflation) affect affordability and market behavior.
- **Building Permits** serve as a leading indicator of supply-side activity.

---

## 📬 Contact

Email : aditivaidya10@gmail.com
