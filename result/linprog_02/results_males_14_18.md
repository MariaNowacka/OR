# LP Results — Males 14 18

**Solver status:** Optimal  
**Minimum lunch cost:** $0.9275 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Cornmeal, Whole Grain, Yellow (dry) | 86.8 | $0.25518 | 27.5% |
| 2 | Milk, 2% Reduced Fat, Fluid | 200.0 | $0.19022 | 20.5% |
| 3 | Cabbage, Green, Raw | 54.8 | $0.09651 | 10.4% |
| 4 | Corn Flakes Cereal (enriched) | 11.8 | $0.09589 | 10.3% |
| 5 | Flaxseeds, Whole | 9.6 | $0.07434 | 8.0% |
| 6 | Milk, Whole (3.25% fat), Fluid | 67.3 | $0.06667 | 7.2% |
| 7 | Vegetable Oil (Soybean/Canola blend) | 17.1 | $0.06045 | 6.5% |
| 8 | Raisin Bran Cereal | 5.2 | $0.03375 | 3.6% |
| 9 | Beef Liver | 3.1 | $0.02761 | 3.0% |
| 10 | Milk, Almond, Unsweetened (fortified) | 12.7 | $0.02340 | 2.5% |
| 11 | Watermelon, Raw | 29.0 | $0.00348 | 0.4% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 750.0000 | 750.000 | 850.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 20.9275 | 15.600 | 18.200 | 5.3275 | -2.7275 |  |
| total_fat_g | 31.1111 | 26.010 | 31.111 | 5.1011 | 0.0000 | [UB] |
| carbohydrates_g | 101.6495 | 39.000 | 45.500 | 62.6495 | -56.1495 |  |
| dietary_fiber_g | 11.4000 | 11.400 | 13.300 | 0.0000 | 1.9000 | [LB] |
| sugars_g | 20.0000 | — | 20.000 | — | -0.0000 | [UB] |
| saturated_fat_g | 6.8269 | — | 8.889 | — | 2.0620 |  |
| monounsaturated_fat_g | 7.2108 | — | — | — | — |  |
| polyunsaturated_fat_g | 14.7036 | — | — | — | — |  |
| cholesterol_mg | 34.9078 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 7.0492 | 3.300 | 3.850 | 3.7492 | -3.1992 |  |
| magnesium_mg | 194.2454 | 123.000 | 143.500 | 71.2454 | -50.7454 |  |
| phosphorus_mg | 577.2436 | 375.000 | 437.500 | 202.2436 | -139.7436 |  |
| potassium_mg | 947.7271 | 900.000 | 1050.000 | 47.7271 | 102.2729 |  |
| sodium_mg | 280.9065 | — | 1280.000 | — | 999.0935 |  |
| zinc_mg | 3.5426 | 3.300 | 3.850 | 0.2426 | 0.3074 |  |
| vitamin_a_ug_rae | 270.0000 | 270.000 | 315.000 | 0.0000 | 45.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_k_ug | 44.4898 | 22.500 | 26.250 | 21.9898 | -18.2398 |  |
| vitamin_c_mg | 22.5000 | 22.500 | 26.250 | 0.0000 | 3.7500 | [LB] |
| thiamin_b1_mg | 0.8650 | 0.360 | 0.420 | 0.5050 | -0.4450 |  |
| riboflavin_b2_mg | 1.0669 | 0.390 | 0.455 | 0.6769 | -0.6119 |  |
| niacin_b3_mg | 7.5683 | 4.800 | 5.600 | 2.7683 | -1.9683 |  |
| vitamin_b6_mg | 1.0041 | 0.390 | 0.455 | 0.6141 | -0.5491 |  |
| folate_ug_dfe | 120.0000 | 120.000 | 140.000 | 0.0000 | 20.0000 | [LB] |
| vitamin_b12_ug | 3.1274 | 0.720 | 0.840 | 2.4074 | -2.2874 |  |
| selenium_ug | 25.5301 | 16.500 | 19.250 | 9.0301 | -6.2801 |  |

## Summary

- **Minimum cost:** $0.9275 per lunch
- **Foods selected:** 11 / 204 available
- **Highest cost item:** Cornmeal, Whole Grain, Yellow (dry)

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
