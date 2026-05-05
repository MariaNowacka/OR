# LP Results — Males 14 18

**Solver status:** Optimal  
**Minimum lunch cost:** $1.0360 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 70.8 | $0.20837 | 20.1% |
| 2 | Salmon, Pink, Canned (drained) | 22.5 | $0.18841 | 18.2% |
| 3 | Collard Greens, Raw | 42.9 | $0.16994 | 16.4% |
| 4 | Milk, 2% Reduced Fat, Fluid | 150.0 | $0.14267 | 13.8% |
| 5 | Whole Chicken (fresh) | 76.5 | $0.11586 | 11.2% |
| 6 | Flaxseeds, Whole | 13.5 | $0.10382 | 10.0% |
| 7 | Sunflower Seeds (kernels, dry-roasted) | 4.8 | $0.03666 | 3.5% |
| 8 | Mayonnaise, Regular | 5.8 | $0.02915 | 2.8% |
| 9 | Watermelon, Raw | 120.0 | $0.01440 | 1.4% |
| 10 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.0% |
| 11 | Beef Liver | 1.0 | $0.00888 | 0.9% |
| 12 | Raisin Bran Cereal | 1.1 | $0.00728 | 0.7% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 750.0000 | 750.000 | 850.000 | -0.0000 | 100.0000 | [LB] |
| protein_g | 42.2625 | 15.600 | 18.200 | 26.6625 | -24.0625 |  |
| total_fat_g | 31.1111 | 26.010 | 31.111 | 5.1011 | 0.0000 | [UB] |
| carbohydrates_g | 79.1862 | 39.000 | 45.500 | 40.1862 | -33.6862 |  |
| dietary_fiber_g | 11.4000 | 11.400 | 13.300 | -0.0000 | 1.9000 | [LB] |
| sugars_g | 16.3306 | — | 20.000 | — | 3.6694 |  |
| saturated_fat_g | 6.8201 | — | 8.889 | — | 2.0688 |  |
| monounsaturated_fat_g | 9.0132 | — | — | — | — |  |
| polyunsaturated_fat_g | 12.5707 | — | — | — | — |  |
| cholesterol_mg | 98.2045 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 5.4841 | 3.300 | 3.850 | 2.1841 | -1.6341 |  |
| magnesium_mg | 214.9514 | 123.000 | 143.500 | 91.9514 | -71.4514 |  |
| phosphorus_mg | 718.5849 | 375.000 | 437.500 | 343.5849 | -281.0849 |  |
| potassium_mg | 1069.1370 | 900.000 | 1050.000 | 169.1370 | -19.1370 |  |
| sodium_mg | 307.4691 | — | 1280.000 | — | 972.5309 |  |
| zinc_mg | 4.8777 | 3.300 | 3.850 | 1.5777 | -1.0277 |  |
| vitamin_a_ug_rae | 270.0000 | 270.000 | 315.000 | 0.0000 | 45.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_k_ug | 190.2684 | 22.500 | 26.250 | 167.7684 | -164.0184 |  |
| vitamin_c_mg | 25.0011 | 22.500 | 26.250 | 2.5011 | 1.2489 |  |
| thiamin_b1_mg | 0.6762 | 0.360 | 0.420 | 0.3162 | -0.2562 |  |
| riboflavin_b2_mg | 0.7183 | 0.390 | 0.455 | 0.3283 | -0.2633 |  |
| niacin_b3_mg | 12.4044 | 4.800 | 5.600 | 7.6044 | -6.8044 |  |
| vitamin_b6_mg | 0.9663 | 0.390 | 0.455 | 0.5763 | -0.5113 |  |
| folate_ug_dfe | 120.0000 | 120.000 | 140.000 | 0.0000 | 20.0000 | [LB] |
| vitamin_b12_ug | 2.3606 | 0.720 | 0.840 | 1.6406 | -1.5206 |  |
| selenium_ug | 43.9527 | 16.500 | 19.250 | 27.4527 | -24.7027 |  |

## Summary

- **Minimum cost:** $1.0360 per lunch
- **Foods selected:** 12 / 204 available
- **Highest cost item:** Cornmeal, Whole Grain, Yellow (dry)

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- dietary_fiber_g
- calcium_mg
- vitamin_a_ug_rae
- vitamin_d_ug
- vitamin_e_mg_ate
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
