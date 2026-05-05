# Dual Simplex Analysis — Females 14 18

**Baseline cost (no group caps):** $0.875591 USD  
**Capped cost (after dual simplex):** $1.019802 USD  
**Cost of acceptability:** +$0.144211 USD (+16.5%)  
**Baseline iterations:** 18  
**Capped iterations:** 31  
**Extra pivots (dual simplex):** +13

## Primal Infeasibility Check (Baseline vs Group Caps)

Positive violation = dual simplex initialisation condition met.

| Group | Cap U_g | Baseline usage | Violation | Primal infeasible |
|-------|--------:|---------------:|----------:|:-----------------:|
| fluid_milk | 150 g | 294.73 g | +144.73 g | YES |
| cooking_oils | 3 g | 20.32 g | +17.32 g | YES |
| grain_products | 120 g | 109.37 g | -10.63 g | no |
| leafy_veg | 80 g | 11.51 g | -68.49 g | no |
| protein_foods | 100 g | 1.14 g | -98.86 g | no |
| fruits | 120 g | 11.58 g | -108.42 g | no |

## Optimal Lunch Menu After Dual Simplex Re-optimisation

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Collard Greens, Raw | 58.7 | $0.23293 | 22.8% |
| 2 | Cornmeal, Whole Grain, Yellow (dry) | 77.2 | $0.22718 | 22.3% |
| 3 | Salmon, Pink, Canned (drained) | 21.4 | $0.17884 | 17.5% |
| 4 | Milk, 2% Reduced Fat, Fluid | 150.0 | $0.14267 | 14.0% |
| 5 | Whole Chicken (fresh) | 78.6 | $0.11912 | 11.7% |
| 6 | Mayonnaise, Regular | 14.1 | $0.07142 | 7.0% |
| 7 | Sunflower Seeds (kernels, dry-roasted) | 2.8 | $0.02153 | 2.1% |
| 8 | Watermelon, Raw | 120.0 | $0.01440 | 1.4% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.0% |
| 10 | Raisin Bran Cereal | 0.2 | $0.00115 | 0.1% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 77.42 g | 42.58 g | OK |
| leafy_veg | 80 g | 58.75 g | 21.25 g | OK |
| protein_foods | 100 g | 100.00 g | 0.00 g | OK |
| fruits | 120 g | 120.00 g | 0.00 g | OK |
