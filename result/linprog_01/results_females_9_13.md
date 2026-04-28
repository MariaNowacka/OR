# LP Results — Females 9 13

**Solver status:** Optimal  
**Minimum lunch cost:** $0.7715 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Milk, 2% Reduced Fat, Fluid | 276.4 | $0.26294 | 34.1% |
| 2 | Cornmeal, Whole Grain, Yellow (dry) | 66.3 | $0.19516 | 25.3% |
| 3 | Corn Flakes Cereal (enriched) | 11.6 | $0.09422 | 12.2% |
| 4 | Collard Greens, Raw | 14.5 | $0.05745 | 7.5% |
| 5 | Vegetable Oil (Soybean/Canola blend) | 14.7 | $0.05173 | 6.7% |
| 6 | Flaxseeds, Whole | 5.6 | $0.04324 | 5.6% |
| 7 | Cabbage, Green, Raw | 22.8 | $0.04013 | 5.2% |
| 8 | Salmon, Pink, Canned (drained) | 1.9 | $0.01599 | 2.1% |
| 9 | Beef Liver | 1.2 | $0.01060 | 1.4% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 600.0000 | 600.000 | 700.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 18.1419 | 10.200 | 11.900 | 7.9419 | -6.2419 |  |
| total_fat_g | 25.2778 | 15.990 | 25.278 | 9.2878 | -0.0000 | [UB] |
| carbohydrates_g | 77.8314 | 39.000 | 45.500 | 38.8314 | -32.3314 |  |
| dietary_fiber_g | 7.8000 | 7.800 | 9.100 | -0.0000 | 1.3000 | [LB] |
| sugars_g | 16.2500 | — | 16.250 | — | -0.0000 | [UB] |
| saturated_fat_g | 5.9685 | — | 7.222 | — | 1.2537 |  |
| monounsaturated_fat_g | 5.9115 | — | — | — | — |  |
| polyunsaturated_fat_g | 11.6216 | — | — | — | — |  |
| cholesterol_mg | 27.7847 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 4.3521 | 2.400 | 2.800 | 1.9521 | -1.5521 |  |
| magnesium_mg | 145.6618 | 72.000 | 84.000 | 73.6618 | -61.6618 |  |
| phosphorus_mg | 488.1664 | 375.000 | 437.500 | 113.1664 | -50.6664 |  |
| potassium_mg | 787.1960 | 690.000 | 805.000 | 97.1960 | 17.8040 |  |
| sodium_mg | 254.7672 | — | 1225.000 | — | 970.2328 |  |
| zinc_mg | 2.7311 | 2.400 | 2.800 | 0.3311 | 0.0689 |  |
| vitamin_a_ug_rae | 180.0000 | 180.000 | 210.000 | 0.0000 | 30.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 3.4365 | 3.300 | 3.850 | 0.1365 | 0.4135 |  |
| vitamin_k_ug | 82.7591 | 18.000 | 21.000 | 64.7591 | -61.7591 |  |
| vitamin_c_mg | 13.5000 | 13.500 | 15.750 | 0.0000 | 2.2500 | [LB] |
| thiamin_b1_mg | 0.6275 | 0.270 | 0.315 | 0.3575 | -0.3125 |  |
| riboflavin_b2_mg | 0.8779 | 0.270 | 0.315 | 0.6079 | -0.5629 |  |
| niacin_b3_mg | 5.5359 | 3.600 | 4.200 | 1.9359 | -1.3359 |  |
| vitamin_b6_mg | 0.8054 | 0.300 | 0.350 | 0.5054 | -0.4554 |  |
| folate_ug_dfe | 90.0000 | 90.000 | 105.000 | 0.0000 | 15.0000 | [LB] |
| vitamin_b12_ug | 2.0571 | 0.540 | 0.630 | 1.5171 | -1.4271 |  |
| selenium_ug | 22.1018 | 12.000 | 14.000 | 10.1017 | -8.1017 |  |

## Summary

- **Minimum cost:** $0.7715 per lunch
- **Foods selected:** 9 / 204 available
- **Highest cost item:** Milk, 2% Reduced Fat, Fluid

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- dietary_fiber_g
- calcium_mg
- vitamin_a_ug_rae
- vitamin_d_ug
- vitamin_c_mg
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
- sugars_g
