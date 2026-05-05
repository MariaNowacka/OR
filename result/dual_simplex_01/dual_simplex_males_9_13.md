# Dual Simplex Analysis — Males 9 13

**Baseline cost (no group caps):** $0.796206 USD  
**Capped cost (after dual simplex):** $0.903599 USD  
**Cost of acceptability:** +$0.107393 USD (+13.5%)  
**Baseline iterations:** 19  
**Capped iterations:** 29  
**Extra pivots (dual simplex):** +10

## Primal Infeasibility Check (Baseline vs Group Caps)

Positive violation = dual simplex initialisation condition met.

| Group | Cap U_g | Baseline usage | Violation | Primal infeasible |
|-------|--------:|---------------:|----------:|:-----------------:|
| fluid_milk | 150 g | 276.37 g | +126.37 g | YES |
| cooking_oils | 3 g | 11.39 g | +8.39 g | YES |
| grain_products | 120 g | 76.44 g | -43.56 g | no |
| leafy_veg | 80 g | 5.44 g | -74.56 g | no |
| protein_foods | 100 g | 2.15 g | -97.85 g | no |
| fruits | 120 g | 0.00 g | -120.00 g | no |

## Optimal Lunch Menu After Dual Simplex Re-optimisation

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Salmon, Pink, Canned (drained) | 23.6 | $0.19719 | 21.8% |
| 2 | Collard Greens, Raw | 38.2 | $0.15133 | 16.7% |
| 3 | Cornmeal, Whole Grain, Yellow (dry) | 45.0 | $0.13224 | 14.6% |
| 4 | Milk, 2% Reduced Fat, Fluid | 136.2 | $0.12955 | 14.3% |
| 5 | Flaxseeds, Whole | 15.1 | $0.11651 | 12.9% |
| 6 | Whole Chicken (fresh) | 76.4 | $0.11580 | 12.8% |
| 7 | Milk, Almond, Unsweetened (fortified) | 13.8 | $0.02549 | 2.8% |
| 8 | Watermelon, Raw | 120.0 | $0.01440 | 1.6% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.2% |
| 10 | Mayonnaise, Regular | 1.7 | $0.00857 | 0.9% |
| 11 | Cheddar Cheese, Natural (sharp) | 0.2 | $0.00193 | 0.2% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 44.96 g | 75.04 g | OK |
| leafy_veg | 80 g | 38.17 g | 41.83 g | OK |
| protein_foods | 100 g | 100.00 g | 0.00 g | OK |
| fruits | 120 g | 120.00 g | 0.00 g | OK |
