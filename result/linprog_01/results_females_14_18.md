# LP Results — Females 14 18

**Solver status:** Optimal  
**Minimum lunch cost:** $0.8724 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Milk, 2% Reduced Fat, Fluid | 300.0 | $0.28534 | 32.7% |
| 2 | Cornmeal, Whole Grain, Yellow (dry) | 91.7 | $0.26956 | 30.9% |
| 3 | Cabbage, Green, Raw | 49.5 | $0.08722 | 10.0% |
| 4 | Vegetable Oil (Soybean/Canola blend) | 21.4 | $0.07556 | 8.7% |
| 5 | Corn Flakes Cereal (enriched) | 7.8 | $0.06348 | 7.3% |
| 6 | Raisin Bran Cereal | 8.8 | $0.05725 | 6.6% |
| 7 | Beef Liver | 2.0 | $0.01789 | 2.0% |
| 8 | Collard Greens, Raw | 3.8 | $0.01515 | 1.7% |
| 9 | Milk, Whole (3.25% fat), Fluid | 0.9 | $0.00091 | 0.1% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 750.0000 | 750.000 | 850.000 | -0.0000 | 100.0000 | [LB] |
| protein_g | 20.3805 | 13.800 | 16.100 | 6.5805 | -4.2805 |  |
| total_fat_g | 31.1111 | 20.010 | 31.111 | 11.1011 | 0.0000 | [UB] |
| carbohydrates_g | 101.1338 | 39.000 | 45.500 | 62.1338 | -55.6338 |  |
| dietary_fiber_g | 9.2611 | 7.800 | 9.100 | 1.4611 | -0.1611 |  |
| sugars_g | 20.0000 | — | 20.000 | — | 0.0000 | [UB] |
| saturated_fat_g | 7.0256 | — | 8.889 | — | 1.8633 |  |
| monounsaturated_fat_g | 7.3997 | — | — | — | — |  |
| polyunsaturated_fat_g | 14.4335 | — | — | — | — |  |
| cholesterol_mg | 31.9853 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | -0.0000 | 65.0000 | [LB] |
| iron_mg | 7.0402 | 4.500 | 5.250 | 2.5402 | -1.7902 |  |
| magnesium_mg | 166.3781 | 108.000 | 126.000 | 58.3781 | -40.3781 |  |
| phosphorus_mg | 562.4452 | 375.000 | 437.500 | 187.4452 | -124.9452 |  |
| potassium_mg | 919.5724 | 690.000 | 805.000 | 229.5724 | -114.5724 |  |
| sodium_mg | 272.2095 | — | 1280.000 | — | 1007.7905 |  |
| zinc_mg | 3.3994 | 2.700 | 3.150 | 0.6994 | -0.2494 |  |
| vitamin_a_ug_rae | 210.0000 | 210.000 | 245.000 | -0.0000 | 35.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 4.5379 | 4.500 | 5.250 | 0.0379 | 0.7121 |  |
| vitamin_k_ug | 57.1579 | 22.500 | 26.250 | 34.6579 | -30.9079 |  |
| vitamin_c_mg | 19.5000 | 19.500 | 22.750 | 0.0000 | 3.2500 | [LB] |
| thiamin_b1_mg | 0.7143 | 0.300 | 0.350 | 0.4143 | -0.3643 |  |
| riboflavin_b2_mg | 1.0633 | 0.300 | 0.350 | 0.7633 | -0.7133 |  |
| niacin_b3_mg | 7.2187 | 4.200 | 4.900 | 3.0187 | -2.3187 |  |
| vitamin_b6_mg | 0.9874 | 0.360 | 0.420 | 0.6274 | -0.5674 |  |
| folate_ug_dfe | 120.0000 | 120.000 | 140.000 | 0.0000 | 20.0000 | [LB] |
| vitamin_b12_ug | 2.5882 | 0.720 | 0.840 | 1.8682 | -1.7482 |  |
| selenium_ug | 24.2345 | 16.500 | 19.250 | 7.7345 | -4.9845 |  |

## Summary

- **Minimum cost:** $0.8724 per lunch
- **Foods selected:** 9 / 204 available
- **Highest cost item:** Milk, 2% Reduced Fat, Fluid

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- calcium_mg
- vitamin_a_ug_rae
- vitamin_d_ug
- vitamin_c_mg
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
- sugars_g
