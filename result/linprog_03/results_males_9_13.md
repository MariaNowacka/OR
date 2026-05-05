# LP Results — Males 9 13

**Solver status:** Optimal  
**Minimum lunch cost:** $0.9036 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Salmon, Pink, Canned (drained) | 23.6 | $0.19719 | 21.8% |
| 2 | Collard Greens, Raw | 38.2 | $0.15133 | 16.8% |
| 3 | Cornmeal, Whole Grain, Yellow (dry) | 45.0 | $0.13224 | 14.6% |
| 4 | Milk, 2% Reduced Fat, Fluid | 136.2 | $0.12955 | 14.3% |
| 5 | Flaxseeds, Whole | 15.1 | $0.11651 | 12.9% |
| 6 | Whole Chicken (fresh) | 76.5 | $0.11580 | 12.8% |
| 7 | Milk, Almond, Unsweetened (fortified) | 13.8 | $0.02549 | 2.8% |
| 8 | Watermelon, Raw | 120.0 | $0.01440 | 1.6% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.2% |
| 10 | Mayonnaise, Regular | 1.7 | $0.00857 | 0.9% |
| 11 | Cheddar Cheese, Natural (sharp) | 0.1 | $0.00193 | 0.2% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 600.0000 | 600.000 | 700.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 38.8616 | 10.200 | 11.900 | 28.6616 | -26.9616 |  |
| total_fat_g | 25.2778 | 18.000 | 25.278 | 7.2778 | -0.0000 | [UB] |
| carbohydrates_g | 56.8685 | 39.000 | 45.500 | 17.8685 | -11.3685 |  |
| dietary_fiber_g | 9.3000 | 9.300 | 10.850 | 0.0000 | 1.5500 | [LB] |
| sugars_g | 15.0520 | — | 16.250 | — | 1.1980 |  |
| saturated_fat_g | 5.8688 | — | 7.222 | — | 1.3534 |  |
| monounsaturated_fat_g | 7.2053 | — | — | — | — |  |
| polyunsaturated_fat_g | 9.9730 | — | — | — | — |  |
| cholesterol_mg | 91.5419 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 4.1252 | 2.400 | 2.800 | 1.7252 | -1.3252 |  |
| magnesium_mg | 179.5666 | 72.000 | 84.000 | 107.5666 | -95.5666 |  |
| phosphorus_mg | 594.9971 | 375.000 | 437.500 | 219.9971 | -157.4971 |  |
| potassium_mg | 943.7205 | 750.000 | 875.000 | 193.7205 | -68.7205 |  |
| sodium_mg | 275.3901 | — | 1225.000 | — | 949.6099 |  |
| zinc_mg | 4.0919 | 2.400 | 2.800 | 1.6919 | -1.2919 |  |
| vitamin_a_ug_rae | 210.4316 | 180.000 | 210.000 | 30.4316 | -0.4316 | [UB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 3.3000 | 3.300 | 3.850 | 0.0000 | 0.5500 | [LB] |
| vitamin_k_ug | 168.6504 | 18.000 | 21.000 | 150.6504 | -147.6504 |  |
| vitamin_c_mg | 23.2693 | 13.500 | 15.750 | 9.7693 | -7.5193 |  |
| thiamin_b1_mg | 0.5790 | 0.270 | 0.315 | 0.3090 | -0.2641 |  |
| riboflavin_b2_mg | 0.5817 | 0.270 | 0.315 | 0.3117 | -0.2667 |  |
| niacin_b3_mg | 10.8537 | 3.600 | 4.200 | 7.2537 | -6.6537 |  |
| vitamin_b6_mg | 0.8012 | 0.300 | 0.350 | 0.5012 | -0.4512 |  |
| folate_ug_dfe | 90.0000 | 90.000 | 105.000 | 0.0000 | 15.0000 | [LB] |
| vitamin_b12_ug | 1.7861 | 0.540 | 0.630 | 1.2461 | -1.1561 |  |
| selenium_ug | 37.3287 | 12.000 | 14.000 | 25.3287 | -23.3287 |  |

## Summary

- **Minimum cost:** $0.9036 per lunch
- **Foods selected:** 11 / 204 available
- **Highest cost item:** Salmon, Pink, Canned (drained)

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- dietary_fiber_g
- calcium_mg
- vitamin_d_ug
- vitamin_e_mg_ate
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
- vitamin_a_ug_rae
