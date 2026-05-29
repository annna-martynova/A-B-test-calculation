# A/B Testing Significance Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/annna-martynova/sales-analysis/blob/main/your_notebook.ipynb)
[![Tableau Dashboard](https://img.shields.io/badge/Tableau-View%20Dashboard-blue?logo=tableau)](https://public.tableau.com/app/profile/anna.martynova/viz/ABTestingSignificanceAnalysis/ABTestingSignificanceAnalysis#2)

## About
Automated A/B testing analysis across multiple metrics and segments \
using Python, with results visualized in Tableau Public.\
Z-test of proportions applied at significance level α = 0.05 \
for control vs. test group comparisons. \

## Tools
SQL, Python (SciPy, Pandas), Tableau Public

## Metrics Tested
- `add_payment_info / session`
- `add_shipping_info / session`
- `begin_checkout / session`
- `new_accounts / session`

Segmented by: device, channel, country, continent

## Results

| Test | Significant Metrics | Outcome |
|------|-------------------|---------|
| Test 1 | 3 out of 4  | Recommend implementation |
| Test 2 | 0 out of 4  | Reject |
| Test 3 | 0 out of 4  | Reject |
| Test 4 | 2 out of 4  | Requires further analysis |

**Test 1** — strongest positive results; all segments show 
significant improvement in 3 key metrics. Ready for rollout.

**Tests 2 & 3** — no statistically significant changes detected. 
Hypotheses not confirmed; changes not recommended for implementation.

**Test 4** — mixed results. Two metrics improved significantly, 
but weaker performance in remaining metrics requires further 
investigation before a decision can be made.

## Recommendations
1. Implement Test 1 changes across all segments
2. Reject Tests 2 and 3
3. Conduct additional refinement and analysis for Test 4

## Dashboard
[View on Tableau Public →](https://public.tableau.com/app/profile/anna.martynova/viz/ABTestingSignificanceAnalysis/ABTestingSignificanceAnalysis#2)
