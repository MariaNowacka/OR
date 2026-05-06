# LP Results — Females 9 13

**Solver status:** Optimal  
**Minimum lunch cost:** $0.9416 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 84.3 | $0.24806 | 26.3% |
| 2 | Salmon, Pink, Canned (drained) | 21.8 | $0.18208 | 19.3% |
| 3 | Collard Greens, Raw | 41.4 | $0.16403 | 17.4% |
| 4 | Milk, 2% Reduced Fat, Fluid | 142.9 | $0.13595 | 14.4% |
| 5 | Cheddar Cheese, Natural (sharp) | 5.8 | $0.07393 | 7.8% |
| 6 | Mayonnaise, Regular | 14.4 | $0.07284 | 7.7% |
| 7 | Flaxseeds, Whole | 5.3 | $0.04099 | 4.3% |
| 8 | Milk, Almond, Unsweetened (fortified) | 7.1 | $0.01305 | 1.4% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.1% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 600.0000 | 600.000 | 700.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 20.3319 | 10.200 | 11.900 | 10.1319 | -8.4319 |  |
| total_fat_g | 25.2778 | 15.990 | 25.278 | 9.2878 | 0.0000 | [UB] |
| carbohydrates_g | 75.8183 | 39.000 | 45.500 | 36.8183 | -30.3183 |  |
| dietary_fiber_g | 9.1179 | 7.800 | 9.100 | 1.3179 | -0.0179 | [UB] |
| sugars_g | 8.2146 | — | 16.250 | — | 8.0354 |  |
| saturated_fat_g | 5.9494 | — | 7.222 | — | 1.2728 |  |
| monounsaturated_fat_g | 6.7156 | — | — | — | — |  |
| polyunsaturated_fat_g | 10.6753 | — | — | — | — |  |
| cholesterol_mg | 37.1304 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 3.7472 | 2.400 | 2.800 | 1.3472 | -0.9472 |  |
| magnesium_mg | 163.3395 | 72.000 | 84.000 | 91.3395 | -79.3395 |  |
| phosphorus_mg | 491.9227 | 375.000 | 437.500 | 116.9227 | -54.4227 |  |
| potassium_mg | 690.0000 | 690.000 | 805.000 | 0.0000 | 115.0000 | [LB] |
| sodium_mg | 329.7140 | — | 1225.000 | — | 895.2860 |  |
| zinc_mg | 2.8751 | 2.400 | 2.800 | 0.4751 | -0.0751 |  |
| vitamin_a_ug_rae | 180.0000 | 180.000 | 210.000 | 0.0000 | 30.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | -0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 3.3000 | 3.300 | 3.850 | 0.0000 | 0.5500 | [LB] |
| vitamin_k_ug | 185.5386 | 18.000 | 21.000 | 167.5386 | -164.5386 |  |
| vitamin_c_mg | 14.6317 | 13.500 | 15.750 | 1.1317 | 1.1183 |  |
| thiamin_b1_mg | 0.4866 | 0.270 | 0.315 | 0.2166 | -0.1716 |  |
| riboflavin_b2_mg | 0.5409 | 0.270 | 0.315 | 0.2709 | -0.2259 |  |
| niacin_b3_mg | 5.5085 | 3.600 | 4.200 | 1.9085 | -1.3085 |  |
| vitamin_b6_mg | 0.5909 | 0.300 | 0.350 | 0.2909 | -0.2409 |  |
| folate_ug_dfe | 90.0000 | 90.000 | 105.000 | 0.0000 | 15.0000 | [LB] |
| vitamin_b12_ug | 1.6042 | 0.540 | 0.630 | 1.0642 | -0.9742 |  |
| selenium_ug | 24.3459 | 12.000 | 14.000 | 12.3459 | -10.3459 |  |

## Summary

- **Minimum cost:** $0.9416 per lunch
- **Foods selected:** 9 / 204 available
- **Highest cost item:** Cornmeal, Whole Grain, Yellow (dry)

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- calcium_mg
- potassium_mg
- vitamin_a_ug_rae
- vitamin_d_ug
- vitamin_e_mg_ate
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
- dietary_fiber_g
