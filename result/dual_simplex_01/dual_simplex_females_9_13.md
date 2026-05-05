# Dual Simplex Analysis — Females 9 13

**Baseline cost (no group caps):** $0.773432 USD  
**Capped cost (after dual simplex):** $0.900184 USD  
**Cost of acceptability:** +$0.126752 USD (+16.4%)  
**Baseline iterations:** 14  
**Capped iterations:** 25  
**Extra pivots (dual simplex):** +11

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
| 1 | Salmon, Pink, Canned (drained) | 23.0 | $0.19248 | 21.4% |
| 2 | Collard Greens, Raw | 41.7 | $0.16540 | 18.4% |
| 3 | Cornmeal, Whole Grain, Yellow (dry) | 46.8 | $0.13774 | 15.3% |
| 4 | Milk, 2% Reduced Fat, Fluid | 139.3 | $0.13253 | 14.7% |
| 5 | Whole Chicken (fresh) | 77.0 | $0.11665 | 13.0% |
| 6 | Flaxseeds, Whole | 8.7 | $0.06692 | 7.4% |
| 7 | Mayonnaise, Regular | 4.4 | $0.02251 | 2.5% |
| 8 | Cheddar Cheese, Natural (sharp) | 1.7 | $0.02128 | 2.4% |
| 9 | Milk, Almond, Unsweetened (fortified) | 10.7 | $0.01970 | 2.2% |
| 10 | Watermelon, Raw | 120.0 | $0.01440 | 1.6% |
| 11 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.2% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 46.83 g | 73.17 g | OK |
| leafy_veg | 80 g | 41.72 g | 38.28 g | OK |
| protein_foods | 100 g | 100.00 g | 0.00 g | OK |
| fruits | 120 g | 120.00 g | 0.00 g | OK |
