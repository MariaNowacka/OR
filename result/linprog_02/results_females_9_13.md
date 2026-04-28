# LP Results — Females 9 13

**Solver status:** Optimal  
**Minimum lunch cost:** $0.7734 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 67.5 | $0.19869 | 25.7% |
| 2 | Milk, 2% Reduced Fat, Fluid | 200.0 | $0.19022 | 24.6% |
| 3 | Corn Flakes Cereal (enriched) | 11.1 | $0.09033 | 11.7% |
| 4 | Milk, Whole (3.25% fat), Fluid | 76.5 | $0.07575 | 9.8% |
| 5 | Collard Greens, Raw | 16.0 | $0.06356 | 8.2% |
| 6 | Vegetable Oil (Soybean/Canola blend) | 13.8 | $0.04852 | 6.3% |
| 7 | Flaxseeds, Whole | 5.3 | $0.04063 | 5.2% |
| 8 | Cabbage, Green, Raw | 21.3 | $0.03754 | 4.8% |
| 9 | Salmon, Pink, Canned (drained) | 2.3 | $0.01914 | 2.5% |
| 10 | Beef Liver | 1.0 | $0.00904 | 1.2% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 600.0000 | 600.000 | 700.000 | -0.0000 | 100.0000 | [LB] |
| protein_g | 18.0507 | 10.200 | 11.900 | 7.8507 | -6.1507 |  |
| total_fat_g | 25.2778 | 15.990 | 25.278 | 9.2878 | 0.0000 | [UB] |
| carbohydrates_g | 78.2489 | 39.000 | 45.500 | 39.2489 | -32.7489 |  |
| dietary_fiber_g | 7.8000 | 7.800 | 9.100 | -0.0000 | 1.3000 | [LB] |
| sugars_g | 16.2500 | — | 16.250 | — | 0.0000 | [UB] |
| saturated_fat_g | 6.3141 | — | 7.222 | — | 0.9081 |  |
| monounsaturated_fat_g | 5.9201 | — | — | — | — |  |
| polyunsaturated_fat_g | 11.0984 | — | — | — | — |  |
| cholesterol_mg | 28.8207 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 4.3095 | 2.400 | 2.800 | 1.9095 | -1.5095 |  |
| magnesium_mg | 145.3409 | 72.000 | 84.000 | 73.3409 | -61.3409 |  |
| phosphorus_mg | 481.2728 | 375.000 | 437.500 | 106.2728 | -43.7728 |  |
| potassium_mg | 776.3686 | 690.000 | 805.000 | 86.3686 | 28.6314 |  |
| sodium_mg | 250.0172 | — | 1225.000 | — | 974.9828 |  |
| zinc_mg | 2.7364 | 2.400 | 2.800 | 0.3364 | 0.0636 |  |
| vitamin_a_ug_rae | 180.0000 | 180.000 | 210.000 | 0.0000 | 30.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 3.3228 | 3.300 | 3.850 | 0.0228 | 0.5272 |  |
| vitamin_k_ug | 88.3686 | 18.000 | 21.000 | 70.3686 | -67.3686 |  |
| vitamin_c_mg | 13.5000 | 13.500 | 15.750 | 0.0000 | 2.2500 | [LB] |
| thiamin_b1_mg | 0.6273 | 0.270 | 0.315 | 0.3573 | -0.3123 |  |
| riboflavin_b2_mg | 0.8671 | 0.270 | 0.315 | 0.5971 | -0.5521 |  |
| niacin_b3_mg | 5.4931 | 3.600 | 4.200 | 1.8931 | -1.2931 |  |
| vitamin_b6_mg | 0.7986 | 0.300 | 0.350 | 0.4986 | -0.4486 |  |
| folate_ug_dfe | 90.0000 | 90.000 | 105.000 | 0.0000 | 15.0000 | [LB] |
| vitamin_b12_ug | 1.9585 | 0.540 | 0.630 | 1.4185 | -1.3285 |  |
| selenium_ug | 22.0960 | 12.000 | 14.000 | 10.0960 | -8.0960 |  |

## Summary

- **Minimum cost:** $0.7734 per lunch
- **Foods selected:** 10 / 204 available
- **Highest cost item:** Cornmeal, Whole Grain, Yellow (dry)

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
