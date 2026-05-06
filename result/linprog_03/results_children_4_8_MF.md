# LP Results — Children 4 8 Mf

**Solver status:** Optimal  
**Minimum lunch cost:** $0.7789 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 73.0 | $0.21458 | 27.6% |
| 2 | Salmon, Pink, Canned (drained) | 22.8 | $0.19048 | 24.5% |
| 3 | Milk, 2% Reduced Fat, Fluid | 150.0 | $0.14267 | 18.3% |
| 4 | Flaxseeds, Whole | 13.4 | $0.10332 | 13.3% |
| 5 | Collard Greens, Raw | 13.0 | $0.05157 | 6.6% |
| 6 | Mayonnaise, Regular | 10.2 | $0.05153 | 6.6% |
| 7 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.4% |
| 8 | Cantaloupe, Raw | 7.7 | $0.00922 | 1.2% |
| 9 | Sunflower Seeds (kernels, dry-roasted) | 0.3 | $0.00245 | 0.3% |
| 10 | Beef Liver | 0.4 | $0.00232 | 0.3% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 550.0000 | 550.000 | 650.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 19.1939 | 5.700 | 6.650 | 13.4939 | -12.5439 |  |
| total_fat_g | 23.3333 | 14.010 | 23.333 | 9.3233 | 0.0000 | [UB] |
| carbohydrates_g | 68.7152 | 39.000 | 45.500 | 29.7152 | -23.2152 |  |
| dietary_fiber_g | 9.5480 | 7.500 | 8.750 | 2.0480 | -0.7980 |  |
| sugars_g | 9.0321 | — | 15.000 | — | 5.9679 |  |
| saturated_fat_g | 4.6925 | — | 6.667 | — | 1.9742 |  |
| monounsaturated_fat_g | 5.8378 | — | — | — | — |  |
| polyunsaturated_fat_g | 11.1958 | — | — | — | — |  |
| cholesterol_mg | 31.2546 | — | — | — | — |  |
| calcium_mg | 300.0000 | 300.000 | 350.000 | 0.0000 | 50.0000 | [LB] |
| iron_mg | 3.6767 | 3.000 | 3.500 | 0.6767 | -0.1767 |  |
| magnesium_mg | 173.1533 | 39.000 | 45.500 | 134.1533 | -127.6533 |  |
| phosphorus_mg | 494.6829 | 150.000 | 175.000 | 344.6829 | -319.6829 |  |
| potassium_mg | 690.0000 | 690.000 | 805.000 | 0.0000 | 115.0000 | [LB] |
| sodium_mg | 265.0115 | — | 1110.000 | — | 844.9885 |  |
| zinc_mg | 2.7925 | 1.500 | 1.750 | 1.2925 | -1.0425 |  |
| vitamin_a_ug_rae | 120.0000 | 120.000 | 140.000 | -0.0000 | 20.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 2.1000 | 2.100 | 2.450 | -0.0000 | 0.3500 | [LB] |
| vitamin_k_ug | 60.8772 | 16.500 | 19.250 | 44.3772 | -41.6272 |  |
| vitamin_c_mg | 7.5000 | 7.500 | 8.750 | -0.0000 | 1.2500 | [LB] |
| thiamin_b1_mg | 0.5623 | 0.180 | 0.210 | 0.3823 | -0.3523 |  |
| riboflavin_b2_mg | 0.5039 | 0.180 | 0.210 | 0.3239 | -0.2939 |  |
| niacin_b3_mg | 5.3139 | 2.400 | 2.800 | 2.9139 | -2.5139 |  |
| vitamin_b6_mg | 0.5553 | 0.180 | 0.210 | 0.3753 | -0.3453 |  |
| folate_ug_dfe | 60.0000 | 60.000 | 70.000 | -0.0000 | 10.0000 | [LB] |
| vitamin_b12_ug | 1.8146 | 0.360 | 0.420 | 1.4546 | -1.3946 |  |
| selenium_ug | 25.3334 | 9.000 | 10.500 | 16.3334 | -14.8334 |  |

## Summary

- **Minimum cost:** $0.7789 per lunch
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
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
