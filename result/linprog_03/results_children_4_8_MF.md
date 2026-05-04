# LP Results — Children 4 8 Mf

**Solver status:** Optimal  
**Minimum lunch cost:** $0.7387 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Salmon, Pink, Canned (drained) | 22.8 | $0.19127 | 25.9% |
| 2 | Milk, 2% Reduced Fat, Fluid | 142.9 | $0.13590 | 18.4% |
| 3 | Whole Chicken (fresh) | 77.2 | $0.11687 | 15.8% |
| 4 | Flaxseeds, Whole | 14.1 | $0.10899 | 14.8% |
| 5 | Cornmeal, Whole Grain, Yellow (dry) | 35.3 | $0.10369 | 14.0% |
| 6 | Raisin Bran Cereal | 4.3 | $0.02813 | 3.8% |
| 7 | Collard Greens, Raw | 3.8 | $0.01510 | 2.0% |
| 8 | Milk, Almond, Unsweetened (fortified) | 7.1 | $0.01315 | 1.8% |
| 9 | Watermelon, Raw | 102.7 | $0.01232 | 1.7% |
| 10 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.4% |
| 11 | Sunflower Seeds (kernels, dry-roasted) | 0.3 | $0.00218 | 0.3% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 550.0000 | 550.000 | 650.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 37.3968 | 5.700 | 6.650 | 31.6968 | -30.7468 |  |
| total_fat_g | 23.3333 | 14.010 | 23.333 | 9.3233 | -0.0000 | [UB] |
| carbohydrates_g | 49.3711 | 39.000 | 45.500 | 10.3711 | -3.8711 |  |
| dietary_fiber_g | 7.5000 | 7.500 | 8.750 | 0.0000 | 1.2500 | [LB] |
| sugars_g | 15.0000 | — | 15.000 | — | -0.0000 | [UB] |
| saturated_fat_g | 5.6552 | — | 6.667 | — | 1.0115 |  |
| monounsaturated_fat_g | 6.7093 | — | — | — | — |  |
| polyunsaturated_fat_g | 8.9416 | — | — | — | — |  |
| cholesterol_mg | 91.2596 | — | — | — | — |  |
| calcium_mg | 300.0000 | 300.000 | 350.000 | 0.0000 | 50.0000 | [LB] |
| iron_mg | 4.7379 | 3.000 | 3.500 | 1.7379 | -1.2379 |  |
| magnesium_mg | 157.1002 | 39.000 | 45.500 | 118.1002 | -111.6002 |  |
| phosphorus_mg | 575.0592 | 150.000 | 175.000 | 425.0592 | -400.0592 |  |
| potassium_mg | 846.7353 | 690.000 | 805.000 | 156.7353 | -41.7353 |  |
| sodium_mg | 266.1404 | — | 1110.000 | — | 843.8596 |  |
| zinc_mg | 3.9214 | 1.500 | 1.750 | 2.4214 | -2.1714 |  |
| vitamin_a_ug_rae | 120.0000 | 120.000 | 140.000 | -0.0000 | 20.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 2.1000 | 2.100 | 2.450 | 0.0000 | 0.3500 | [LB] |
| vitamin_k_ug | 18.1544 | 16.500 | 19.250 | 1.6544 | 1.0956 |  |
| vitamin_c_mg | 9.7384 | 7.500 | 8.750 | 2.2384 | -0.9884 |  |
| thiamin_b1_mg | 0.5618 | 0.180 | 0.210 | 0.3818 | -0.3518 |  |
| riboflavin_b2_mg | 0.6008 | 0.180 | 0.210 | 0.4208 | -0.3908 |  |
| niacin_b3_mg | 10.9782 | 2.400 | 2.800 | 8.5782 | -8.1782 |  |
| vitamin_b6_mg | 0.7930 | 0.180 | 0.210 | 0.6130 | -0.5830 |  |
| folate_ug_dfe | 60.0000 | 60.000 | 70.000 | -0.0000 | 10.0000 | [LB] |
| vitamin_b12_ug | 1.7633 | 0.360 | 0.420 | 1.4033 | -1.3433 |  |
| selenium_ug | 37.2255 | 9.000 | 10.500 | 28.2255 | -26.7255 |  |

## Summary

- **Minimum cost:** $0.7387 per lunch
- **Foods selected:** 11 / 204 available
- **Highest cost item:** Salmon, Pink, Canned (drained)

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
- sugars_g
