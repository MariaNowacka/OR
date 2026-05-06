# Dual Simplex Analysis — Children 4 8 Mf

**Baseline cost (no group caps):** $0.692458 USD  
**Capped cost (after dual simplex):** $0.778860 USD  
**Cost of acceptability:** +$0.086402 USD (+12.5%)  
**Baseline iterations:** 22  
**Capped iterations:** 36  
**Extra pivots (dual simplex):** +14

## Primal Infeasibility Check (Baseline vs Group Caps)

Positive violation = dual simplex initialisation condition met.

| Group | Cap U_g | Baseline usage | Violation | Primal infeasible |
|-------|--------:|---------------:|----------:|:-----------------:|
| fluid_milk | 150 g | 260.50 g | +110.50 g | YES |
| cooking_oils | 3 g | 11.13 g | +8.13 g | YES |
| grain_products | 120 g | 69.07 g | -50.93 g | no |
| leafy_veg | 80 g | 0.00 g | -80.00 g | no |
| protein_foods | 100 g | 8.23 g | -91.77 g | no |
| fruits | 120 g | 1.25 g | -118.75 g | no |

## Optimal Lunch Menu After Dual Simplex Re-optimisation

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 73.0 | $0.21458 | 27.6% |
| 2 | Salmon, Pink, Canned (drained) | 22.7 | $0.19048 | 24.5% |
| 3 | Milk, 2% Reduced Fat, Fluid | 150.0 | $0.14267 | 18.3% |
| 4 | Flaxseeds, Whole | 13.4 | $0.10332 | 13.3% |
| 5 | Collard Greens, Raw | 13.0 | $0.05157 | 6.6% |
| 6 | Mayonnaise, Regular | 10.2 | $0.05153 | 6.6% |
| 7 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.4% |
| 8 | Cantaloupe, Raw | 7.7 | $0.00922 | 1.2% |
| 9 | Sunflower Seeds (kernels, dry-roasted) | 0.3 | $0.00245 | 0.3% |
| 10 | Beef Liver | 0.4 | $0.00232 | 0.3% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 72.96 g | 47.04 g | OK |
| leafy_veg | 80 g | 13.01 g | 66.99 g | OK |
| protein_foods | 100 g | 23.17 g | 76.83 g | OK |
| fruits | 120 g | 7.68 g | 112.32 g | OK |
