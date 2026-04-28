# LP Results — Males 9 13

**Solver status:** Optimal  
**Minimum lunch cost:** $0.7962 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Milk, 2% Reduced Fat, Fluid | 200.0 | $0.19022 | 23.9% |
| 2 | Cornmeal, Whole Grain, Yellow (dry) | 63.3 | $0.18629 | 23.4% |
| 3 | Corn Flakes Cereal (enriched) | 13.1 | $0.10684 | 13.4% |
| 4 | Flaxseeds, Whole | 12.0 | $0.09284 | 11.7% |
| 5 | Milk, Whole (3.25% fat), Fluid | 66.2 | $0.06563 | 8.2% |
| 6 | Cabbage, Green, Raw | 31.4 | $0.05535 | 7.0% |
| 7 | Vegetable Oil (Soybean/Canola blend) | 11.4 | $0.04013 | 5.0% |
| 8 | Collard Greens, Raw | 5.4 | $0.02156 | 2.7% |
| 9 | Milk, Almond, Unsweetened (fortified) | 10.1 | $0.01873 | 2.4% |
| 10 | Beef Liver | 1.4 | $0.01251 | 1.6% |
| 11 | Salmon, Pink, Canned (drained) | 0.7 | $0.00610 | 0.8% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 600.0000 | 600.000 | 700.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 18.4106 | 10.200 | 11.900 | 8.2106 | -6.5106 |  |
| total_fat_g | 25.2778 | 18.000 | 25.278 | 7.2778 | 0.0000 | [UB] |
| carbohydrates_g | 78.2360 | 39.000 | 45.500 | 39.2360 | -32.7360 |  |
| dietary_fiber_g | 9.3000 | 9.300 | 10.850 | 0.0000 | 1.5500 | [LB] |
| sugars_g | 16.2500 | — | 16.250 | — | 0.0000 | [UB] |
| saturated_fat_g | 6.0521 | — | 7.222 | — | 1.1701 |  |
| monounsaturated_fat_g | 5.7955 | — | — | — | — |  |
| polyunsaturated_fat_g | 11.5643 | — | — | — | — |  |
| cholesterol_mg | 28.5233 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 4.8228 | 2.400 | 2.800 | 2.4228 | -2.0228 |  |
| magnesium_mg | 164.4708 | 72.000 | 84.000 | 92.4708 | -80.4708 |  |
| phosphorus_mg | 505.7297 | 375.000 | 437.500 | 130.7297 | -68.2297 |  |
| potassium_mg | 804.4339 | 750.000 | 875.000 | 54.4339 | 70.5661 |  |
| sodium_mg | 261.2312 | — | 1225.000 | — | 963.7688 |  |
| zinc_mg | 2.9059 | 2.400 | 2.800 | 0.5059 | -0.1059 |  |
| vitamin_a_ug_rae | 180.0000 | 180.000 | 210.000 | 0.0000 | 30.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 3.3000 | 3.300 | 3.850 | -0.0000 | 0.5500 | [LB] |
| vitamin_k_ug | 49.8428 | 18.000 | 21.000 | 31.8428 | -28.8428 |  |
| vitamin_c_mg | 13.5000 | 13.500 | 15.750 | 0.0000 | 2.2500 | [LB] |
| thiamin_b1_mg | 0.7455 | 0.270 | 0.315 | 0.4755 | -0.4305 |  |
| riboflavin_b2_mg | 0.8928 | 0.270 | 0.315 | 0.6228 | -0.5778 |  |
| niacin_b3_mg | 5.7860 | 3.600 | 4.200 | 2.1860 | -1.5860 |  |
| vitamin_b6_mg | 0.8386 | 0.300 | 0.350 | 0.5386 | -0.4886 |  |
| folate_ug_dfe | 90.0000 | 90.000 | 105.000 | 0.0000 | 15.0000 | [LB] |
| vitamin_b12_ug | 2.1252 | 0.540 | 0.630 | 1.5852 | -1.4952 |  |
| selenium_ug | 23.0782 | 12.000 | 14.000 | 11.0782 | -9.0782 |  |

## Summary

- **Minimum cost:** $0.7962 per lunch
- **Foods selected:** 11 / 204 available
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
