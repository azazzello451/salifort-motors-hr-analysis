# Salifort Motors — HR Attrition Analysis

Salifort Motors was losing 1 in 6 employees. This project finds out why — and predicts who's next.

---

## What I did

- Explored HR survey data (11,991 employees) to identify attrition drivers
- Built and compared 4 ML models; selected Random Forest (AUC 0.987)
- Generated a per-employee risk report with predicted leaving probability and plain-text risk explanations
- Built an interactive Power BI dashboard for HR decision-makers

---

## Key findings

- **Satisfaction** is the #1 predictor — leavers score 25 points lower than stayers
- **Year 3–5** is the critical window — turnover peaks at 45% in year 5
- **Two leaver profiles**: burned-out (low satisfaction, pushed out) vs. high-performers (pulled away by better offers)
- **Workload sweet spot**: 160–240 hrs/month — below or above, attrition climbs fast
- **Low earners leave at 4× the rate** of high earners

---

## Results

| Model | AUC |
|-------|-----|
| Logistic Regression | 0.837 |
| Decision Tree | 0.977 |
| **Random Forest** ✅ | **0.987** |
| XGBoost | 0.985 |

---

## Files

| File | Description |
|------|-------------|
| `Salifort_Motors_Final.ipynb` | Full analysis & model |
| `HR_capstone_dataset.csv` | Raw dataset |
| `salifort_complete_report.csv` | Per-employee risk report |
| `capstone_dashboard.pbix` | Power BI dashboard |

---

## Stack

![Python](https://img.shields.io/badge/Python-3.10-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-2.0-green)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)

---

```bash
git clone https://github.com/azazzello451/salifort-motors-hr-analysis.git
pip install -r requirements.txt
jupyter notebook Salifort_Motors_Final.ipynb
```
