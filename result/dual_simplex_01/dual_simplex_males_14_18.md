# Dual Simplex Analysis — Males 14 18

**Baseline cost (no group caps):** $0.918707 USD  
**Capped cost (after dual simplex):** $1.085043 USD  
**Cost of acceptability:** +$0.166336 USD (+18.1%)  
**Baseline iterations:** 20  
**Capped iterations:** 35  
**Extra pivots (dual simplex):** +15

## Primal Infeasibility Check (Baseline vs Group Caps)

Positive violation = dual simplex initialisation condition met.

| Group | Cap U_g | Baseline usage | Violation | Primal infeasible |
|-------|--------:|---------------:|----------:|:-----------------:|
| fluid_milk | 150 g | 289.29 g | +139.29 g | YES |
| cooking_oils | 3 g | 14.68 g | +11.68 g | YES |
| grain_products | 120 g | 101.88 g | -18.12 g | no |
| leafy_veg | 80 g | 0.00 g | -80.00 g | no |
| protein_foods | 100 g | 2.88 g | -97.12 g | no |
| fruits | 120 g | 16.25 g | -103.75 g | no |

## Optimal Lunch Menu After Dual Simplex Re-optimisation

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 108.1 | $0.31790 | 29.3% |
| 2 | Collard Greens, Raw | 52.5 | $0.20820 | 19.2% |
| 3 | Salmon, Pink, Canned (drained) | 21.4 | $0.17915 | 16.5% |
| 4 | Milk, 2% Reduced Fat, Fluid | 150.0 | $0.14267 | 13.1% |
| 5 | Mayonnaise, Regular | 18.2 | $0.09251 | 8.5% |
| 6 | Flaxseeds, Whole | 10.9 | $0.08410 | 7.8% |
| 7 | Sunflower Seeds (kernels, dry-roasted) | 2.9 | $0.02274 | 2.1% |
| 8 | Sweet Potato, Baked with Skin | 6.9 | $0.01897 | 1.7% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.0% |
| 10 | Cantaloupe, Raw | 6.9 | $0.00823 | 0.8% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 108.08 g | 11.92 g | OK |
| leafy_veg | 80 g | 52.51 g | 27.49 g | OK |
| protein_foods | 100 g | 21.40 g | 78.60 g | OK |
| fruits | 120 g | 6.86 g | 113.14 g | OK |
