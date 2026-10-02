# Supplier Risk Scoring Model
## Automated Supplier Risk Assessment and Early Warning System

### Project Overview
Machine learning supplier risk scoring model that automatically
scores every supplier on a 0 to 100 risk scale and flags
suppliers showing deteriorating performance before they
cause operational disruptions.

**Tools:** Python, Pandas, NumPy, Matplotlib, Scikit-learn,
Jupyter Notebook
**Dataset:** DataCo Smart Supply Chain Dataset (Kaggle)
**Scale:** 51 suppliers scored | 180,519 orders analysed

---

### Risk Scoring Dashboard
![Supplier Risk Dashboard](supplier_risk_dashboard.png)

---

### How the Risk Model Works

The model scores each supplier across 5 weighted dimensions:

| Dimension | Weight | What It Measures |
|-----------|--------|-----------------|
| Late Delivery Rate | 35% | Most critical — direct customer impact |
| Delivery Day Variance | 25% | How far actual vs scheduled days drift |
| Profit Margin Risk | 20% | Low margin suppliers are higher risk |
| Discount Dependency | 10% | Heavy discounting signals instability |
| Cancellation Rate | 10% | Order cancellations signal relationship risk |

Each dimension is normalised to 0 to 100 then combined
using the weighted average to produce a final risk score.

---

### Risk Level Classification

| Risk Level | Score Range | Action Required |
|------------|-------------|-----------------|
| CRITICAL | 75 to 100 | Immediate intervention |
| HIGH | 60 to 74 | Weekly monitoring |
| MEDIUM | 45 to 59 | Monthly review |
| LOW | 0 to 44 | Quarterly check-in |

---

### Key Findings

**Risk Scorecard Results:**
- Critical Risk suppliers: 0
- High Risk suppliers: 5
- Medium Risk suppliers: 42
- Low Risk suppliers: 4
- Average risk score: 53.8

**Top 3 Highest Risk Suppliers:**
1. Strength Training — Score 67.8 — Late delivery 57.7%
2. As Seen on TV — Score 67.1 — Late delivery 57.4%
3. Pet Supplies — Score 66.4 — Late delivery 58.9%

**Best Performing Supplier:**
Men's Golf Clubs — Score 30.8 — Late delivery only 47.7%
Recommended as benchmark for supplier excellence program.

---

### Early Warning System
![Early Warning System](early_warning_system.png)

The early warning system compares supplier performance
across two consecutive 3-month periods and automatically
flags suppliers showing deterioration.

**Most Critical Alert:**
Baby category supplier showed a 16.5 percentage point
increase in late delivery rate AND a 14.7 percentage
point margin decline simultaneously — indicating an
urgent procurement intervention is needed.

**Alert Summary:**
- Suppliers monitored: 7
- Suppliers flagged: 6
- Critical alerts: 1
- High alerts: 3
- Watch alerts: 2
- Stable suppliers: 1

---

### Recommendations

1. **IMMEDIATE** — Review Baby and Cameras supplier contracts.
   Both showing critical simultaneous deterioration
   in delivery performance and profit margin.

2. **HIGH** — Put Strength Training and As Seen on TV
   on weekly performance monitoring programme.

3. **MEDIUM** — Establish monthly scorecard reviews
   for all 42 medium risk suppliers with
   defined improvement targets.

4. **BENCHMARK** — Use Men's Golf Clubs process
   as template for supplier excellence programme.

5. **SYSTEM** — Run this early warning model weekly
   to catch deterioration signals before they
   become delivery crises.

---

### How to Run

1. Clone this repository
2. Install: pip install pandas numpy matplotlib
   seaborn scikit-learn jupyter
3. Open: jupyter notebook
4. Run: Supplier_Risk_Scoring_Model.ipynb

---

### About
Portfolio project by Sankruth Sriram — Supply Chain
and Operations Analytics Professional based in Berlin.

LinkedIn: linkedin.com/in/sankruth-sriram
GitHub: github.com/xhamaniksanta
