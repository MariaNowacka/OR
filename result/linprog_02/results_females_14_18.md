# LP Results — Females 14 18

**Solver status:** Optimal  
**Minimum lunch cost:** $0.8756 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 92.6 | $0.27226 | 31.1% |
| 2 | Milk, 2% Reduced Fat, Fluid | 200.0 | $0.19022 | 21.7% |
| 3 | Milk, Whole (3.25% fat), Fluid | 94.7 | $0.09385 | 10.7% |
| 4 | Corn Flakes Cereal (enriched) | 9.2 | $0.07459 | 8.5% |
| 5 | Vegetable Oil (Soybean/Canola blend) | 20.3 | $0.07161 | 8.2% |
| 6 | Cabbage, Green, Raw | 30.5 | $0.05376 | 6.1% |
| 7 | Raisin Bran Cereal | 7.7 | $0.04969 | 5.7% |
| 8 | Collard Greens, Raw | 11.5 | $0.04565 | 5.2% |
| 9 | Cantaloupe, Raw | 11.6 | $0.01390 | 1.6% |
| 10 | Beef Liver | 1.1 | $0.01007 | 1.1% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 750.0000 | 750.000 | 850.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 19.8854 | 13.800 | 16.100 | 6.0854 | -3.7854 |  |
| total_fat_g | 31.1111 | 20.010 | 31.111 | 11.1011 | 0.0000 | [UB] |
| carbohydrates_g | 102.0740 | 39.000 | 45.500 | 63.0740 | -56.5740 |  |
| dietary_fiber_g | 9.1460 | 7.800 | 9.100 | 1.3460 | -0.0460 |  |
| sugars_g | 20.0000 | — | 20.000 | — | -0.0000 | [UB] |
| saturated_fat_g | 7.3665 | — | 8.889 | — | 1.5224 |  |
| monounsaturated_fat_g | 7.3935 | — | — | — | — |  |
| polyunsaturated_fat_g | 13.8818 | — | — | — | — |  |
| cholesterol_mg | 29.9139 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 6.8243 | 4.500 | 5.250 | 2.3243 | -1.5743 |  |
| magnesium_mg | 166.0260 | 108.000 | 126.000 | 58.0260 | -40.0260 |  |
| phosphorus_mg | 541.2676 | 375.000 | 437.500 | 166.2676 | -103.7676 |  |
| potassium_mg | 903.6099 | 690.000 | 805.000 | 213.6099 | -98.6099 |  |
| sodium_mg | 270.8412 | — | 1280.000 | — | 1009.1588 |  |
| zinc_mg | 3.3301 | 2.700 | 3.150 | 0.6301 | -0.1801 |  |
| vitamin_a_ug_rae | 210.0000 | 210.000 | 245.000 | 0.0000 | 35.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 4.5000 | 4.500 | 5.250 | -0.0000 | 0.7500 | [LB] |
| vitamin_k_ug | 76.5773 | 22.500 | 26.250 | 54.0773 | -50.3273 |  |
| vitamin_c_mg | 19.5000 | 19.500 | 22.750 | -0.0000 | 3.2500 | [LB] |
| thiamin_b1_mg | 0.7261 | 0.300 | 0.350 | 0.4261 | -0.3761 |  |
| riboflavin_b2_mg | 1.0304 | 0.300 | 0.350 | 0.7304 | -0.6804 |  |
| niacin_b3_mg | 7.2396 | 4.200 | 4.900 | 3.0396 | -2.3396 |  |
| vitamin_b6_mg | 0.9861 | 0.360 | 0.420 | 0.6261 | -0.5661 |  |
| folate_ug_dfe | 120.0000 | 120.000 | 140.000 | -0.0000 | 20.0000 | [LB] |
| vitamin_b12_ug | 2.0238 | 0.720 | 0.840 | 1.3038 | -1.1838 |  |
| selenium_ug | 23.8759 | 16.500 | 19.250 | 7.3759 | -4.6259 |  |

## Summary

- **Minimum cost:** $0.8756 per lunch
- **Foods selected:** 10 / 204 available
- **Highest cost item:** Cornmeal, Whole Grain, Yellow (dry)

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- calcium_mg
- vitamin_a_ug_rae
- vitamin_d_ug
- vitamin_e_mg_ate
- vitamin_c_mg
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
- sugars_g
