# LP Results — Females 9 13

**Solver status:** Optimal  
**Minimum lunch cost:** $0.9002 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Salmon, Pink, Canned (drained) | 23.0 | $0.19248 | 21.4% |
| 2 | Collard Greens, Raw | 41.7 | $0.16540 | 18.4% |
| 3 | Cornmeal, Whole Grain, Yellow (dry) | 46.8 | $0.13774 | 15.3% |
| 4 | Milk, 2% Reduced Fat, Fluid | 139.3 | $0.13253 | 14.7% |
| 5 | Whole Chicken (fresh) | 77.0 | $0.11665 | 13.0% |
| 6 | Flaxseeds, Whole | 8.7 | $0.06692 | 7.4% |
| 7 | Mayonnaise, Regular | 4.4 | $0.02251 | 2.5% |
| 8 | Cheddar Cheese, Natural (sharp) | 1.7 | $0.02128 | 2.4% |
| 9 | Milk, Almond, Unsweetened (fortified) | 10.7 | $0.01970 | 2.2% |
| 10 | Watermelon, Raw | 120.0 | $0.01440 | 1.6% |
| 11 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.2% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 600.0000 | 600.000 | 700.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 38.4661 | 10.200 | 11.900 | 28.2661 | -26.5661 |  |
| total_fat_g | 25.2778 | 15.990 | 25.278 | 9.2878 | -0.0000 | [UB] |
| carbohydrates_g | 56.8181 | 39.000 | 45.500 | 17.8181 | -11.3181 |  |
| dietary_fiber_g | 7.8000 | 7.800 | 9.100 | -0.0000 | 1.3000 | [LB] |
| sugars_g | 15.1597 | — | 16.250 | — | 1.0903 |  |
| saturated_fat_g | 6.3013 | — | 7.222 | — | 0.9209 |  |
| monounsaturated_fat_g | 7.4733 | — | — | — | — |  |
| polyunsaturated_fat_g | 9.2186 | — | — | — | — |  |
| cholesterol_mg | 95.1626 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 3.8547 | 2.400 | 2.800 | 1.4547 | -1.0547 |  |
| magnesium_mg | 158.2861 | 72.000 | 84.000 | 86.2861 | -74.2861 |  |
| phosphorus_mg | 568.9882 | 375.000 | 437.500 | 193.9882 | -131.4882 |  |
| potassium_mg | 909.4197 | 690.000 | 805.000 | 219.4197 | -104.4197 |  |
| sodium_mg | 299.1442 | — | 1225.000 | — | 925.8558 |  |
| zinc_mg | 3.9328 | 2.400 | 2.800 | 1.5328 | -1.1328 |  |
| vitamin_a_ug_rae | 223.1170 | 180.000 | 210.000 | 43.1170 | -13.1170 |  |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 3.3000 | 3.300 | 3.850 | 0.0000 | 0.5500 | [LB] |
| vitamin_k_ug | 184.6179 | 18.000 | 21.000 | 166.6179 | -163.6179 |  |
| vitamin_c_mg | 24.4897 | 13.500 | 15.750 | 10.9897 | -8.7397 |  |
| thiamin_b1_mg | 0.4850 | 0.270 | 0.315 | 0.2150 | -0.1700 |  |
| riboflavin_b2_mg | 0.5913 | 0.270 | 0.315 | 0.3213 | -0.2763 |  |
| niacin_b3_mg | 10.7572 | 3.600 | 4.200 | 7.1572 | -6.5572 |  |
| vitamin_b6_mg | 0.7898 | 0.300 | 0.350 | 0.4898 | -0.4398 |  |
| folate_ug_dfe | 90.0000 | 90.000 | 105.000 | 0.0000 | 15.0000 | [LB] |
| vitamin_b12_ug | 1.7901 | 0.540 | 0.630 | 1.2501 | -1.1601 |  |
| selenium_ug | 36.2668 | 12.000 | 14.000 | 24.2668 | -22.2668 |  |

## Summary

- **Minimum cost:** $0.9002 per lunch
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
