# LP Results — Males 14 18

**Solver status:** Optimal  
**Minimum lunch cost:** $0.9256 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Milk, 2% Reduced Fat, Fluid | 267.6 | $0.25452 | 27.5% |
| 2 | Cornmeal, Whole Grain, Yellow (dry) | 85.8 | $0.25238 | 27.3% |
| 3 | Corn Flakes Cereal (enriched) | 12.1 | $0.09834 | 10.6% |
| 4 | Cabbage, Green, Raw | 54.5 | $0.09596 | 10.4% |
| 5 | Flaxseeds, Whole | 10.0 | $0.07696 | 8.3% |
| 6 | Vegetable Oil (Soybean/Canola blend) | 17.9 | $0.06319 | 6.8% |
| 7 | Raisin Bran Cereal | 5.0 | $0.03236 | 3.5% |
| 8 | Beef Liver | 3.2 | $0.02865 | 3.1% |
| 9 | Milk, Almond, Unsweetened (fortified) | 10.6 | $0.01960 | 2.1% |
| 10 | Watermelon, Raw | 30.4 | $0.00365 | 0.4% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 750.0000 | 750.000 | 850.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 21.0836 | 15.600 | 18.200 | 5.4836 | -2.8836 |  |
| total_fat_g | 31.1111 | 26.010 | 31.111 | 5.1011 | -0.0000 | [UB] |
| carbohydrates_g | 101.2068 | 39.000 | 45.500 | 62.2068 | -55.7068 |  |
| dietary_fiber_g | 11.4000 | 11.400 | 13.300 | -0.0000 | 1.9000 | [LB] |
| sugars_g | 20.0000 | — | 20.000 | — | 0.0000 | [UB] |
| saturated_fat_g | 6.5282 | — | 8.889 | — | 2.3607 |  |
| monounsaturated_fat_g | 7.1940 | — | — | — | — |  |
| polyunsaturated_fat_g | 15.1649 | — | — | — | — |  |
| cholesterol_mg | 34.0451 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 7.0170 | 3.300 | 3.850 | 3.7170 | -3.1670 |  |
| magnesium_mg | 194.8885 | 123.000 | 143.500 | 71.8885 | -51.3885 |  |
| phosphorus_mg | 584.0821 | 375.000 | 437.500 | 209.0821 | -146.5821 |  |
| potassium_mg | 958.2512 | 900.000 | 1050.000 | 58.2512 | 91.7488 |  |
| sodium_mg | 283.6730 | — | 1280.000 | — | 996.3270 |  |
| zinc_mg | 3.5372 | 3.300 | 3.850 | 0.2372 | 0.3128 |  |
| vitamin_a_ug_rae | 270.0000 | 270.000 | 315.000 | 0.0000 | 45.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_k_ug | 44.2499 | 22.500 | 26.250 | 21.7499 | -17.9999 |  |
| vitamin_c_mg | 22.5000 | 22.500 | 26.250 | 0.0000 | 3.7500 | [LB] |
| thiamin_b1_mg | 0.8621 | 0.360 | 0.420 | 0.5021 | -0.4421 |  |
| riboflavin_b2_mg | 1.0717 | 0.390 | 0.455 | 0.6817 | -0.6167 |  |
| niacin_b3_mg | 7.5802 | 4.800 | 5.600 | 2.7802 | -1.9802 |  |
| vitamin_b6_mg | 1.0060 | 0.390 | 0.455 | 0.6160 | -0.5510 |  |
| folate_ug_dfe | 120.0000 | 120.000 | 140.000 | -0.0000 | 20.0000 | [LB] |
| vitamin_b12_ug | 3.1979 | 0.720 | 0.840 | 2.4779 | -2.3579 |  |
| selenium_ug | 25.6107 | 16.500 | 19.250 | 9.1107 | -6.3607 |  |

## Summary

- **Minimum cost:** $0.9256 per lunch
- **Foods selected:** 10 / 204 available
- **Highest cost item:** Milk, 2% Reduced Fat, Fluid

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- dietary_fiber_g
- calcium_mg
- vitamin_a_ug_rae
- vitamin_d_ug
- vitamin_e_mg_ate
- vitamin_c_mg
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
- sugars_g
