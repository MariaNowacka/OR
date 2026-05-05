# LP Results — Males 14 18

**Solver status:** Optimal  
**Minimum lunch cost:** $1.0850 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 108.1 | $0.31790 | 29.3% |
| 2 | Collard Greens, Raw | 52.5 | $0.20821 | 19.2% |
| 3 | Salmon, Pink, Canned (drained) | 21.4 | $0.17915 | 16.5% |
| 4 | Milk, 2% Reduced Fat, Fluid | 150.0 | $0.14267 | 13.2% |
| 5 | Mayonnaise, Regular | 18.2 | $0.09251 | 8.5% |
| 6 | Flaxseeds, Whole | 10.9 | $0.08410 | 7.8% |
| 7 | Sunflower Seeds (kernels, dry-roasted) | 3.0 | $0.02274 | 2.1% |
| 8 | Sweet Potato, Baked with Skin | 6.9 | $0.01897 | 1.8% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.0% |
| 10 | Cantaloupe, Raw | 6.9 | $0.00823 | 0.8% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 750.0000 | 750.000 | 850.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 23.0759 | 15.600 | 18.200 | 7.4759 | -4.8759 |  |
| total_fat_g | 31.1111 | 26.010 | 31.111 | 5.1011 | 0.0000 | [UB] |
| carbohydrates_g | 99.2686 | 39.000 | 45.500 | 60.2686 | -53.7686 |  |
| dietary_fiber_g | 13.2989 | 11.400 | 13.300 | 1.8989 | 0.0011 | [UB] |
| sugars_g | 9.9560 | — | 20.000 | — | 10.0440 |  |
| saturated_fat_g | 5.8769 | — | 8.889 | — | 3.0120 |  |
| monounsaturated_fat_g | 8.2065 | — | — | — | — |  |
| polyunsaturated_fat_g | 14.7855 | — | — | — | — |  |
| cholesterol_mg | 33.5193 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 5.0715 | 3.300 | 3.850 | 1.7715 | -1.2215 |  |
| magnesium_mg | 223.5145 | 123.000 | 143.500 | 100.5145 | -80.0145 |  |
| phosphorus_mg | 601.6134 | 375.000 | 437.500 | 226.6134 | -164.1134 |  |
| potassium_mg | 900.0000 | 900.000 | 1050.000 | 0.0000 | 150.0000 | [LB] |
| sodium_mg | 330.9801 | — | 1280.000 | — | 949.0199 |  |
| zinc_mg | 3.6225 | 3.300 | 3.850 | 0.3225 | 0.2275 |  |
| vitamin_a_ug_rae | 270.0000 | 270.000 | 315.000 | 0.0000 | 45.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_k_ug | 235.6981 | 22.500 | 26.250 | 213.1981 | -209.4481 |  |
| vitamin_c_mg | 22.5000 | 22.500 | 26.250 | 0.0000 | 3.7500 | [LB] |
| thiamin_b1_mg | 0.6861 | 0.360 | 0.420 | 0.3261 | -0.2661 |  |
| riboflavin_b2_mg | 0.6094 | 0.390 | 0.455 | 0.2194 | -0.1544 |  |
| niacin_b3_mg | 6.9637 | 4.800 | 5.600 | 2.1637 | -1.3637 |  |
| vitamin_b6_mg | 0.7673 | 0.390 | 0.455 | 0.3773 | -0.3123 |  |
| folate_ug_dfe | 123.3915 | 120.000 | 140.000 | 3.3915 | 16.6085 |  |
| vitamin_b12_ug | 1.5261 | 0.720 | 0.840 | 0.8061 | -0.6861 |  |
| selenium_ug | 29.8690 | 16.500 | 19.250 | 13.3690 | -10.6190 |  |

## Summary

- **Minimum cost:** $1.0850 per lunch
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
- dietary_fiber_g
