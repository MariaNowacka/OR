# Dual Simplex Analysis — Males 9 13

**Baseline cost (no group caps):** $0.791513 USD  
**Capped cost (after dual simplex):** $0.948933 USD  
**Cost of acceptability:** +$0.157420 USD (+19.9%)  
**Baseline iterations:** 27  
**Capped iterations:** 37  
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
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 80.9 | $0.23808 | 25.1% |
| 2 | Salmon, Pink, Canned (drained) | 22.6 | $0.18918 | 19.9% |
| 3 | Collard Greens, Raw | 38.0 | $0.15070 | 15.9% |
| 4 | Milk, 2% Reduced Fat, Fluid | 138.9 | $0.13212 | 13.9% |
| 5 | Flaxseeds, Whole | 15.3 | $0.11821 | 12.5% |
| 6 | Mayonnaise, Regular | 10.2 | $0.05177 | 5.5% |
| 7 | Cheddar Cheese, Natural (sharp) | 2.8 | $0.03586 | 3.8% |
| 8 | Milk, Almond, Unsweetened (fortified) | 11.1 | $0.02050 | 2.2% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.1% |
| 10 | Beef Liver | 0.3 | $0.00193 | 0.2% |

## Group Cap Feasibility After Dual Simplex

| Group | Cap U_g | Usage | Slack | Primal feasible |
|-------|--------:|------:|------:|:---------------:|
| fluid_milk | 150 g | 150.00 g | 0.00 g | OK |
| cooking_oils | 3 g | 3.00 g | 0.00 g | OK |
| grain_products | 120 g | 80.95 g | 39.05 g | OK |
| leafy_veg | 80 g | 38.01 g | 41.99 g | OK |
| protein_foods | 100 g | 22.94 g | 77.06 g | OK |
| fruits | 120 g | 0.00 g | 120.00 g | OK |
