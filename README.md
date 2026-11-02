# Commercial Pricing & Sensitivity Analysis Model

An executive-level Excel model designed to analyze portfolio margins, conduct variance analysis, and stress-test net profit against market price and cost shifts.

---

## Project Overview

This project builds a aggregate baseline model for a commercial payment portfolio to evaluate overall revenue realization, cost variances, and profit resilience under varying market conditions.

---

## Key Baseline Metrics


| **Baseline Revenue** | €403.67 |
| **Baseline Direct Cost** | €235.37 |
| **Baseline Net Profit** | €168.30 |
| **Baseline Net Margin** | ~41.69% |

---

## Key Features

* **Baseline Financial Aggregation:** Summarized transactional data using dynamic Excel functions (`SUM`, `SUMIFS`).
* **Variance Analysis:** Analyzed price and cost variances to identify commercial margin leakage across customer groups.
* **Sensitivity Modeling:** Built dynamic one-way sensitivity tables using absolute cell references (`$B$1`, `$B$2`) to test:
  * **Price Realization Shifts:** `-0.50%` to `+0.50%`
  * **Supplier Cost Shifts:** `-0.25%` to `+0.25%`

---

## Key Formulas Used

* **Net Profit:** `= B1 - B2`
* **Adjusted Revenue:** `= $B$1 * (1 + Shift%)`
* **Adjusted Net Profit (Price Shift):** `= Adjusted_Revenue - $B$2`
* **Adjusted Net Profit (Cost Shift):** `= $B$1 - ($B$2 * (1 + Shift%))`

---

## Tools & Tech

* **Software:** Microsoft Excel
* **Skills:** Financial Modeling, Sensitivity Analysis, Variance Analysis, Scenario Modeling