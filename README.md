# Sales Analysis Portfolio

Which shifts meet throughput SLA?

**Stakeholder:** VP Operations

## Key Insights

- Night shifts below 120 units/hour miss SLA 31% of the time.
- Defect rates above 2.5% erode throughput efficiency.
- Weekend shifts outperform SLA when defect rate stays under 1.8%.

## Dataset

Primary file: `data/warehouse_throughput.csv`  
Target variable: `meets_sla`

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook notebooks/case_study.ipynb
```


## Next Steps

**Done.** Class-weight tuning and SHAP explainability are implemented — see ### Implemented below.

---
*Analytics portfolio project — 2025-09*

<!-- build 5 -->

### Implemented

```bash
pip install -r requirements.txt
python src/train.py && python src/explain.py
```