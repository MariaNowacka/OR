# Dual Simplex Analysis — Males 14 18

**Baseline cost (no group caps):** $0.927501 USD  
**Capped cost (after dual simplex):** $1.036012 USD  
**Cost of acceptability:** +$0.108511 USD (+11.7%)  
**Baseline iterations:** 19  
**Capped iterations:** 27  
**Extra pivots (dual simplex):** +8

## Primal Infeasibility Check (Baseline vs Group Caps)

Positive violation = dual simplex initialisation condition met.

| Group | Cap U_g | Baseline usage | Violation | Primal infeasible |
|-------|--------:|---------------:|----------:|:-----------------:|
| fluid_milk | 150 g | 279.95 g | +129.95 g | YES |
| cooking_oils | 3 g | 17.15 g | +14.15 g | YES |
| grain_products | 120 g | 103.72 g | -16.28 g | no |
| leafy_veg | 80 g | 0.00 g | -80.00 g | no |
| protein_foods | 100 g | 3.13 g | -96.87 g | no |
| fruits | 120 g | 29.04 g | -90.96 g | no |

## Optimal Lunch Menu After Dual Simplex Re-optimisation

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 70.8 | $0.20837 | 20.1% |
| 2 | Salmon, Pink, Canned (drained) | 22.5 | $0.18841 | 18.2% |
| 3 | Collard Greens, Raw | 42.9 | $0.16994 | 16.4% |
| 4 | Milk, 2% Reduced Fat, Fluid | 150.0 | $0.14267 | 13.8% |
| 5 | Whole Chicken (fresh) | 76.5 | $0.11586 | 11.2% |
| 6 | Flaxseeds, Whole | 13.5 | $0.10382 | 10.0% |
| 7 | Sunflower Seeds (kernels, dry-roasted) | 4.8 | $0.03666 | 3.5% |
| 8 | Mayonnaise, Regular | 5.7 | $0.02915 | 2.8% |
| 9 | Watermelon, Raw | 120.0 | $0.01440 | 1.4% |
| 10 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.0% |
| 11 | Beef Liver | 1.0 | $0.00888 | 0.9% |
| 12 | Raisin Bran Cereal | 1.1 | $0.00728 | 0.7% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 71.97 g | 48.03 g | OK |
| leafy_veg | 80 g | 42.86 g | 37.14 g | OK |
| protein_foods | 100 g | 100.00 g | 0.00 g | OK |
| fruits | 120 g | 120.00 g | 0.00 g | OK |
