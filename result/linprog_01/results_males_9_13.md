# LP Results — Males 9 13

**Solver status:** Optimal  
**Minimum lunch cost:** $0.7941 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Milk, 2% Reduced Fat, Fluid | 267.3 | $0.25419 | 32.0% |
| 2 | Cornmeal, Whole Grain, Yellow (dry) | 62.5 | $0.18389 | 23.2% |
| 3 | Corn Flakes Cereal (enriched) | 13.2 | $0.10717 | 13.5% |
| 4 | Flaxseeds, Whole | 12.3 | $0.09485 | 11.9% |
| 5 | Cabbage, Green, Raw | 31.9 | $0.05629 | 7.1% |
| 6 | Vegetable Oil (Soybean/Canola blend) | 12.2 | $0.04286 | 5.4% |
| 7 | Collard Greens, Raw | 4.9 | $0.01932 | 2.4% |
| 8 | Milk, Almond, Unsweetened (fortified) | 8.2 | $0.01524 | 1.9% |
| 9 | Beef Liver | 1.6 | $0.01381 | 1.7% |
| 10 | Salmon, Pink, Canned (drained) | 0.8 | $0.00652 | 0.8% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 600.0000 | 600.000 | 700.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 18.5918 | 10.200 | 11.900 | 8.3918 | -6.6918 |  |
| total_fat_g | 25.2778 | 18.000 | 25.278 | 7.2778 | -0.0000 | [UB] |
| carbohydrates_g | 77.7608 | 39.000 | 45.500 | 38.7608 | -32.2608 |  |
| dietary_fiber_g | 9.3000 | 9.300 | 10.850 | 0.0000 | 1.5500 | [LB] |
| sugars_g | 16.2500 | — | 16.250 | — | 0.0000 | [UB] |
| saturated_fat_g | 5.7676 | — | 7.222 | — | 1.4546 |  |
| monounsaturated_fat_g | 5.7824 | — | — | — | — |  |
| polyunsaturated_fat_g | 12.0065 | — | — | — | — |  |
| cholesterol_mg | 27.8799 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 4.8198 | 2.400 | 2.800 | 2.4198 | -2.0198 |  |
| magnesium_mg | 165.0548 | 72.000 | 84.000 | 93.0548 | -81.0548 |  |
| phosphorus_mg | 513.6750 | 375.000 | 437.500 | 138.6750 | -76.1750 |  |
| potassium_mg | 815.6864 | 750.000 | 875.000 | 65.6864 | 59.3136 |  |
| sodium_mg | 263.5350 | — | 1225.000 | — | 961.4650 |  |
| zinc_mg | 2.9098 | 2.400 | 2.800 | 0.5098 | -0.1098 |  |
| vitamin_a_ug_rae | 180.0000 | 180.000 | 210.000 | 0.0000 | 30.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 3.3000 | 3.300 | 3.850 | 0.0000 | 0.5500 | [LB] |
| vitamin_k_ug | 47.7771 | 18.000 | 21.000 | 29.7770 | -26.7770 |  |
| vitamin_c_mg | 13.5000 | 13.500 | 15.750 | 0.0000 | 2.2500 | [LB] |
| thiamin_b1_mg | 0.7411 | 0.270 | 0.315 | 0.4711 | -0.4261 |  |
| riboflavin_b2_mg | 0.8985 | 0.270 | 0.315 | 0.6285 | -0.5835 |  |
| niacin_b3_mg | 5.7959 | 3.600 | 4.200 | 2.1959 | -1.5959 |  |
| vitamin_b6_mg | 0.8405 | 0.300 | 0.350 | 0.5405 | -0.4905 |  |
| folate_ug_dfe | 90.0000 | 90.000 | 105.000 | 0.0000 | 15.0000 | [LB] |
| vitamin_b12_ug | 2.2190 | 0.540 | 0.630 | 1.6790 | -1.5890 |  |
| selenium_ug | 23.1872 | 12.000 | 14.000 | 11.1872 | -9.1872 |  |

## Summary

- **Minimum cost:** $0.7941 per lunch
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
