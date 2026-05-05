# Dual Simplex Analysis — Children 4 8 Mf

**Baseline cost (no group caps):** $0.687245 USD  
**Capped cost (after dual simplex):** $0.738656 USD  
**Cost of acceptability:** +$0.051411 USD (+7.5%)  
**Baseline iterations:** 19  
**Capped iterations:** 28  
**Extra pivots (dual simplex):** +9

## Primal Infeasibility Check (Baseline vs Group Caps)

Positive violation = dual simplex initialisation condition met.

| Group | Cap U_g | Baseline usage | Violation | Primal infeasible |
|-------|--------:|---------------:|----------:|:-----------------:|
| fluid_milk | 150 g | 198.87 g | +48.87 g | YES |
| cooking_oils | 3 g | 12.67 g | +9.67 g | YES |
| grain_products | 120 g | 69.41 g | -50.59 g | no |
| leafy_veg | 80 g | 2.34 g | -77.66 g | no |
| protein_foods | 100 g | 13.14 g | -86.86 g | no |
| fruits | 120 g | 56.00 g | -64.00 g | no |

## Optimal Lunch Menu After Dual Simplex Re-optimisation

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Salmon, Pink, Canned (drained) | 22.8 | $0.19127 | 25.9% |
| 2 | Milk, 2% Reduced Fat, Fluid | 142.9 | $0.13590 | 18.4% |
| 3 | Whole Chicken (fresh) | 77.2 | $0.11687 | 15.8% |
| 4 | Flaxseeds, Whole | 14.1 | $0.10899 | 14.8% |
| 5 | Cornmeal, Whole Grain, Yellow (dry) | 35.3 | $0.10369 | 14.0% |
| 6 | Raisin Bran Cereal | 4.3 | $0.02813 | 3.8% |
| 7 | Collard Greens, Raw | 3.8 | $0.01510 | 2.0% |
| 8 | Milk, Almond, Unsweetened (fortified) | 7.1 | $0.01315 | 1.8% |
| 9 | Watermelon, Raw | 102.7 | $0.01233 | 1.7% |
| 10 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.4% |
| 11 | Sunflower Seeds (kernels, dry-roasted) | 0.3 | $0.00218 | 0.3% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 39.59 g | 80.41 g | OK |
| leafy_veg | 80 g | 3.81 g | 76.19 g | OK |
| protein_foods | 100 g | 100.00 g | 0.00 g | OK |
| fruits | 120 g | 102.71 g | 17.29 g | OK |
