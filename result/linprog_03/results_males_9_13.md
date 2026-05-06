# LP Results — Males 9 13

**Solver status:** Optimal  
**Minimum lunch cost:** $0.9489 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 81.0 | $0.23808 | 25.1% |
| 2 | Salmon, Pink, Canned (drained) | 22.6 | $0.18918 | 19.9% |
| 3 | Collard Greens, Raw | 38.0 | $0.15070 | 15.9% |
| 4 | Milk, 2% Reduced Fat, Fluid | 138.9 | $0.13212 | 13.9% |
| 5 | Flaxseeds, Whole | 15.3 | $0.11821 | 12.5% |
| 6 | Mayonnaise, Regular | 10.2 | $0.05177 | 5.5% |
| 7 | Cheddar Cheese, Natural (sharp) | 2.8 | $0.03586 | 3.8% |
| 8 | Milk, Almond, Unsweetened (fortified) | 11.1 | $0.02050 | 2.2% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.1% |
| 10 | Beef Liver | 0.3 | $0.00193 | 0.2% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 600.0000 | 600.000 | 700.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 21.1612 | 10.200 | 11.900 | 10.9612 | -9.2612 |  |
| total_fat_g | 25.2778 | 18.000 | 25.278 | 7.2778 | -0.0000 | [UB] |
| carbohydrates_g | 75.6930 | 39.000 | 45.500 | 36.6930 | -30.1930 |  |
| dietary_fiber_g | 11.4933 | 9.300 | 10.850 | 2.1933 | -0.6433 |  |
| sugars_g | 8.0935 | — | 16.250 | — | 8.1565 |  |
| saturated_fat_g | 5.2151 | — | 7.222 | — | 2.0071 |  |
| monounsaturated_fat_g | 6.3064 | — | — | — | — |  |
| polyunsaturated_fat_g | 11.9087 | — | — | — | — |  |
| cholesterol_mg | 33.0073 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 4.1875 | 2.400 | 2.800 | 1.7875 | -1.3875 |  |
| magnesium_mg | 196.5642 | 72.000 | 84.000 | 124.5642 | -112.5642 |  |
| phosphorus_mg | 532.5579 | 375.000 | 437.500 | 157.5579 | -95.0579 |  |
| potassium_mg | 750.0000 | 750.000 | 875.000 | 0.0000 | 125.0000 | [LB] |
| sodium_mg | 290.5180 | — | 1225.000 | — | 934.4820 |  |
| zinc_mg | 3.1374 | 2.400 | 2.800 | 0.7374 | -0.3374 |  |
| vitamin_a_ug_rae | 180.0000 | 180.000 | 210.000 | 0.0000 | 30.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 3.3000 | 3.300 | 3.850 | -0.0000 | 0.5500 | [LB] |
| vitamin_k_ug | 170.1466 | 18.000 | 21.000 | 152.1466 | -149.1466 |  |
| vitamin_c_mg | 13.5000 | 13.500 | 15.750 | 0.0000 | 2.2500 | [LB] |
| thiamin_b1_mg | 0.6341 | 0.270 | 0.315 | 0.3641 | -0.3191 |  |
| riboflavin_b2_mg | 0.5386 | 0.270 | 0.315 | 0.2686 | -0.2236 |  |
| niacin_b3_mg | 5.7781 | 3.600 | 4.200 | 2.1781 | -1.5781 |  |
| vitamin_b6_mg | 0.6190 | 0.300 | 0.350 | 0.3190 | -0.2690 |  |
| folate_ug_dfe | 93.4442 | 90.000 | 105.000 | 3.4442 | 11.5558 |  |
| vitamin_b12_ug | 1.7881 | 0.540 | 0.630 | 1.2481 | -1.1581 |  |
| selenium_ug | 26.1808 | 12.000 | 14.000 | 14.1808 | -12.1808 |  |

## Summary

- **Minimum cost:** $0.9489 per lunch
- **Foods selected:** 10 / 204 available
- **Highest cost item:** Cornmeal, Whole Grain, Yellow (dry)

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- calcium_mg
- potassium_mg
- vitamin_a_ug_rae
- vitamin_d_ug
- vitamin_e_mg_ate
- vitamin_c_mg

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
