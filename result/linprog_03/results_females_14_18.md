# LP Results — Females 14 18

**Solver status:** Optimal  
**Minimum lunch cost:** $1.0610 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 116.9 | $0.34380 | 32.4% |
| 2 | Collard Greens, Raw | 62.3 | $0.24705 | 23.3% |
| 3 | Salmon, Pink, Canned (drained) | 20.1 | $0.16789 | 15.8% |
| 4 | Milk, 2% Reduced Fat, Fluid | 140.2 | $0.13339 | 12.6% |
| 5 | Mayonnaise, Regular | 25.8 | $0.13082 | 12.3% |
| 6 | Milk, Almond, Unsweetened (fortified) | 9.8 | $0.01803 | 1.7% |
| 7 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.0% |
| 8 | Cheddar Cheese, Natural (sharp) | 0.7 | $0.00941 | 0.9% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 750.0000 | 750.000 | 850.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 21.0183 | 13.800 | 16.100 | 7.2183 | -4.9183 |  |
| total_fat_g | 31.1111 | 20.010 | 31.111 | 11.1011 | 0.0000 | [UB] |
| carbohydrates_g | 100.3964 | 39.000 | 45.500 | 61.3964 | -54.8964 |  |
| dietary_fiber_g | 10.8056 | 7.800 | 9.100 | 3.0056 | -1.7056 |  |
| sugars_g | 8.3916 | — | 20.000 | — | 11.6084 |  |
| saturated_fat_g | 6.2575 | — | 8.889 | — | 2.6314 |  |
| monounsaturated_fat_g | 8.6308 | — | — | — | — |  |
| polyunsaturated_fat_g | 13.9719 | — | — | — | — |  |
| cholesterol_mg | 37.1228 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 4.6626 | 4.500 | 5.250 | 0.1626 | 0.5874 |  |
| magnesium_mg | 187.7245 | 108.000 | 126.000 | 79.7245 | -61.7245 |  |
| phosphorus_mg | 509.0856 | 375.000 | 437.500 | 134.0856 | -71.5856 |  |
| potassium_mg | 775.6199 | 690.000 | 805.000 | 85.6199 | 29.3801 |  |
| sodium_mg | 377.3216 | — | 1280.000 | — | 902.6784 |  |
| zinc_mg | 3.1590 | 2.700 | 3.150 | 0.4590 | -0.0090 | [UB] |
| vitamin_a_ug_rae | 227.9106 | 210.000 | 245.000 | 17.9106 | 17.0894 |  |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 4.5000 | 4.500 | 5.250 | -0.0000 | 0.7500 | [LB] |
| vitamin_k_ug | 279.6003 | 22.500 | 26.250 | 257.1003 | -253.3503 |  |
| vitamin_c_mg | 21.9961 | 19.500 | 22.750 | 2.4961 | 0.7539 |  |
| thiamin_b1_mg | 0.5309 | 0.300 | 0.350 | 0.2309 | -0.1809 |  |
| riboflavin_b2_mg | 0.5952 | 0.300 | 0.350 | 0.2952 | -0.2452 |  |
| niacin_b3_mg | 6.5541 | 4.200 | 4.900 | 2.3541 | -1.6541 |  |
| vitamin_b6_mg | 0.7022 | 0.360 | 0.420 | 0.3422 | -0.2822 |  |
| folate_ug_dfe | 120.0000 | 120.000 | 140.000 | 0.0000 | 20.0000 | [LB] |
| vitamin_b12_ug | 1.4860 | 0.720 | 0.840 | 0.7660 | -0.6460 |  |
| selenium_ug | 25.2574 | 16.500 | 19.250 | 8.7574 | -6.0074 |  |

## Summary

- **Minimum cost:** $1.0610 per lunch
- **Foods selected:** 8 / 204 available
- **Highest cost item:** Cornmeal, Whole Grain, Yellow (dry)

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- calcium_mg
- vitamin_d_ug
- vitamin_e_mg_ate
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
- zinc_mg
