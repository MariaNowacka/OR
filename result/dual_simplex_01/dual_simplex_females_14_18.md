# Dual Simplex Analysis — Females 14 18

**Baseline cost (no group caps):** $0.870636 USD  
**Capped cost (after dual simplex):** $1.060968 USD  
**Cost of acceptability:** +$0.190332 USD (+21.9%)  
**Baseline iterations:** 18  
**Capped iterations:** 27  
**Extra pivots (dual simplex):** +9

## Primal Infeasibility Check (Baseline vs Group Caps)

Positive violation = dual simplex initialisation condition met.

| Group | Cap U_g | Baseline usage | Violation | Primal infeasible |
|-------|--------:|---------------:|----------:|:-----------------:|
| fluid_milk | 150 g | 301.86 g | +151.86 g | YES |
| cooking_oils | 3 g | 20.14 g | +17.14 g | YES |
| grain_products | 120 g | 109.23 g | -10.77 g | no |
| leafy_veg | 80 g | 4.31 g | -75.69 g | no |
| protein_foods | 100 g | 1.83 g | -98.17 g | no |
| fruits | 120 g | 0.00 g | -120.00 g | no |

## Optimal Lunch Menu After Dual Simplex Re-optimisation

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 116.9 | $0.34380 | 32.4% |
| 2 | Collard Greens, Raw | 62.3 | $0.24705 | 23.3% |
| 3 | Salmon, Pink, Canned (drained) | 20.1 | $0.16789 | 15.8% |
| 4 | Milk, 2% Reduced Fat, Fluid | 140.2 | $0.13339 | 12.6% |
| 5 | Mayonnaise, Regular | 25.8 | $0.13082 | 12.3% |
| 6 | Milk, Almond, Unsweetened (fortified) | 9.8 | $0.01803 | 1.7% |
| 7 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.0% |
| 8 | Cheddar Cheese, Natural (sharp) | 0.7 | $0.00941 | 0.9% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 116.89 g | 3.11 g | OK |
| leafy_veg | 80 g | 62.31 g | 17.69 g | OK |
| protein_foods | 100 g | 20.05 g | 79.95 g | OK |
| fruits | 120 g | 0.00 g | 120.00 g | OK |
