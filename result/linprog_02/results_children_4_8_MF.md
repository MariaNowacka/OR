# LP Results — Children 4 8 Mf

**Solver status:** Optimal  
**Minimum lunch cost:** $0.6872 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Milk, 2% Reduced Fat, Fluid | 198.9 | $0.18915 | 27.5% |
| 2 | Cornmeal, Whole Grain, Yellow (dry) | 60.6 | $0.17824 | 25.9% |
| 3 | Salmon, Pink, Canned (drained) | 12.5 | $0.10467 | 15.2% |
| 4 | Corn Flakes Cereal (enriched) | 8.8 | $0.07184 | 10.4% |
| 5 | Flaxseeds, Whole | 8.7 | $0.06698 | 9.8% |
| 6 | Vegetable Oil (Soybean/Canola blend) | 12.7 | $0.04466 | 6.5% |
| 7 | Cabbage, Green, Raw | 5.7 | $0.01003 | 1.5% |
| 8 | Collard Greens, Raw | 2.3 | $0.00927 | 1.4% |
| 9 | Watermelon, Raw | 56.0 | $0.00672 | 1.0% |
| 10 | Beef Liver | 0.6 | $0.00568 | 0.8% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 550.0000 | 550.000 | 650.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 17.3241 | 5.700 | 6.650 | 11.6241 | -10.6741 |  |
| total_fat_g | 23.3333 | 14.010 | 23.333 | 9.3233 | -0.0000 | [UB] |
| carbohydrates_g | 70.8123 | 39.000 | 45.500 | 31.8123 | -25.3123 |  |
| dietary_fiber_g | 7.5000 | 7.500 | 8.750 | 0.0000 | 1.2500 | [LB] |
| sugars_g | 15.0000 | — | 15.000 | — | 0.0000 | [UB] |
| saturated_fat_g | 4.9163 | — | 6.667 | — | 1.7504 |  |
| monounsaturated_fat_g | 5.4242 | — | — | — | — |  |
| polyunsaturated_fat_g | 11.3099 | — | — | — | — |  |
| cholesterol_mg | 24.9153 | — | — | — | — |  |
| calcium_mg | 300.0000 | 300.000 | 350.000 | 0.0000 | 50.0000 | [LB] |
| iron_mg | 4.0271 | 3.000 | 3.500 | 1.0271 | -0.5271 |  |
| magnesium_mg | 144.6352 | 39.000 | 45.500 | 105.6352 | -99.1352 |  |
| phosphorus_mg | 451.9046 | 150.000 | 175.000 | 301.9045 | -276.9045 |  |
| potassium_mg | 700.9791 | 690.000 | 805.000 | 10.9791 | 104.0209 |  |
| sodium_mg | 237.1940 | — | 1110.000 | — | 872.8060 |  |
| zinc_mg | 2.4797 | 1.500 | 1.750 | 0.9797 | -0.7297 |  |
| vitamin_a_ug_rae | 120.0000 | 120.000 | 140.000 | 0.0000 | 20.0000 | [LB] |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 2.8775 | 2.100 | 2.450 | 0.7775 | -0.4275 |  |
| vitamin_k_ug | 16.5000 | 16.500 | 19.250 | -0.0000 | 2.7500 | [LB] |
| vitamin_c_mg | 7.5000 | 7.500 | 8.750 | 0.0000 | 1.2500 | [LB] |
| thiamin_b1_mg | 0.5885 | 0.180 | 0.210 | 0.4085 | -0.3785 |  |
| riboflavin_b2_mg | 0.6865 | 0.180 | 0.210 | 0.5065 | -0.4765 |  |
| niacin_b3_mg | 5.5694 | 2.400 | 2.800 | 3.1694 | -2.7694 |  |
| vitamin_b6_mg | 0.6553 | 0.180 | 0.210 | 0.4753 | -0.4453 |  |
| folate_ug_dfe | 60.0000 | 60.000 | 70.000 | -0.0000 | 10.0000 | [LB] |
| vitamin_b12_ug | 1.7695 | 0.360 | 0.420 | 1.4095 | -1.3495 |  |
| selenium_ug | 22.3111 | 9.000 | 10.500 | 13.3111 | -11.8111 |  |

## Summary

- **Minimum cost:** $0.6872 per lunch
- **Foods selected:** 10 / 204 available
- **Highest cost item:** Milk, 2% Reduced Fat, Fluid

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- dietary_fiber_g
- calcium_mg
- vitamin_a_ug_rae
- vitamin_d_ug
- vitamin_k_ug
- vitamin_c_mg
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
- sugars_g
