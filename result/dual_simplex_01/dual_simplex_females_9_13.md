# Dual Simplex Analysis — Females 9 13

**Baseline cost (no group caps):** $0.770043 USD  
**Capped cost (after dual simplex):** $0.941642 USD  
**Cost of acceptability:** +$0.171599 USD (+22.3%)  
**Baseline iterations:** 19  
**Capped iterations:** 29  
**Extra pivots (dual simplex):** +10

## Primal Infeasibility Check (Baseline vs Group Caps)

Positive violation = dual simplex initialisation condition met.

| Group | Cap U_g | Baseline usage | Violation | Primal infeasible |
|-------|--------:|---------------:|----------:|:-----------------:|
| fluid_milk | 150 g | 276.46 g | +126.46 g | YES |
| cooking_oils | 3 g | 13.77 g | +10.77 g | YES |
| grain_products | 120 g | 78.63 g | -41.37 g | no |
| leafy_veg | 80 g | 16.03 g | -63.97 g | no |
| protein_foods | 100 g | 3.31 g | -96.69 g | no |
| fruits | 120 g | 0.00 g | -120.00 g | no |

## Optimal Lunch Menu After Dual Simplex Re-optimisation

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 84.3 | $0.24806 | 26.3% |
| 2 | Salmon, Pink, Canned (drained) | 21.7 | $0.18208 | 19.3% |
| 3 | Collard Greens, Raw | 41.4 | $0.16403 | 17.4% |
| 4 | Milk, 2% Reduced Fat, Fluid | 142.9 | $0.13595 | 14.4% |
| 5 | Cheddar Cheese, Natural (sharp) | 5.8 | $0.07393 | 7.9% |
| 6 | Mayonnaise, Regular | 14.4 | $0.07284 | 7.7% |
| 7 | Flaxseeds, Whole | 5.3 | $0.04100 | 4.4% |
| 8 | Milk, Almond, Unsweetened (fortified) | 7.1 | $0.01305 | 1.4% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.1% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 84.34 g | 35.66 g | OK |
| leafy_veg | 80 g | 41.37 g | 38.63 g | OK |
| protein_foods | 100 g | 21.77 g | 78.23 g | OK |
| fruits | 120 g | 0.00 g | 120.00 g | OK |
