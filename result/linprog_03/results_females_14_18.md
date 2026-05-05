# LP Results — Females 14 18

**Solver status:** Optimal  
**Minimum lunch cost:** $1.0198 USD

## Optimal Lunch Foods

The LP selected these foods and gram quantities to satisfy all nutritional constraints at the lowest possible cost.

| # | Food | Portion (g) | Cost (USD) | Cost share (%) |
|---|------|------------:|------------:|---------------:|
| 1 | Collard Greens, Raw | 58.8 | $0.23293 | 22.8% |
| 2 | Cornmeal, Whole Grain, Yellow (dry) | 77.2 | $0.22718 | 22.3% |
| 3 | Salmon, Pink, Canned (drained) | 21.4 | $0.17884 | 17.5% |
| 4 | Milk, 2% Reduced Fat, Fluid | 150.0 | $0.14267 | 14.0% |
| 5 | Whole Chicken (fresh) | 78.6 | $0.11912 | 11.7% |
| 6 | Mayonnaise, Regular | 14.1 | $0.07142 | 7.0% |
| 7 | Sunflower Seeds (kernels, dry-roasted) | 2.8 | $0.02152 | 2.1% |
| 8 | Watermelon, Raw | 120.0 | $0.01440 | 1.4% |
| 9 | Vegetable Oil (Soybean/Canola blend) | 3.0 | $0.01057 | 1.0% |
| 10 | Raisin Bran Cereal | 0.2 | $0.00115 | 0.1% |

## Nutritional Achievement vs. DRI Bounds

- **LB slack** = achieved - lower bound (0 = binding constraint)  
- **UB slack** = upper bound - achieved (0 = binding constraint)  
- **[LB] / [UB]** marks binding constraints — these are the cost drivers.

| Nutrient | Achieved | LB | UB | LB slack | UB slack | Binding |
|----------|--------:|----:|----:|---------:|---------:|---------|
| energy_kcal | 750.0000 | 750.000 | 850.000 | 0.0000 | 100.0000 | [LB] |
| protein_g | 40.4671 | 13.800 | 16.100 | 26.6671 | -24.3671 |  |
| total_fat_g | 31.1111 | 20.010 | 31.111 | 11.1011 | 0.0000 | [UB] |
| carbohydrates_g | 79.9539 | 39.000 | 45.500 | 40.9539 | -34.4539 |  |
| dietary_fiber_g | 8.4929 | 7.800 | 9.100 | 0.6929 | 0.6071 |  |
| sugars_g | 16.0306 | — | 20.000 | — | 3.9694 |  |
| saturated_fat_g | 7.2688 | — | 8.889 | — | 1.6201 |  |
| monounsaturated_fat_g | 9.5720 | — | — | — | — |  |
| polyunsaturated_fat_g | 11.5475 | — | — | — | — |  |
| cholesterol_mg | 100.3355 | — | — | — | — |  |
| calcium_mg | 390.0000 | 390.000 | 455.000 | 0.0000 | 65.0000 | [LB] |
| iron_mg | 4.6545 | 4.500 | 5.250 | 0.1545 | 0.5955 |  |
| magnesium_mg | 171.3631 | 108.000 | 126.000 | 63.3631 | -45.3631 |  |
| phosphorus_mg | 622.5393 | 375.000 | 437.500 | 247.5393 | -185.0393 |  |
| potassium_mg | 993.3724 | 690.000 | 805.000 | 303.3724 | -188.3724 |  |
| sodium_mg | 354.0809 | — | 1280.000 | — | 925.9191 |  |
| zinc_mg | 4.3504 | 2.700 | 3.150 | 1.6504 | -1.2004 |  |
| vitamin_a_ug_rae | 263.8772 | 210.000 | 245.000 | 53.8772 | -18.8772 |  |
| vitamin_d_ug | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_e_mg_ate | 4.5000 | 4.500 | 5.250 | 0.0000 | 0.7500 | [LB] |
| vitamin_k_ug | 261.1429 | 22.500 | 26.250 | 238.6429 | -234.8929 |  |
| vitamin_c_mg | 30.4976 | 19.500 | 22.750 | 10.9976 | -7.7476 |  |
| thiamin_b1_mg | 0.4750 | 0.300 | 0.350 | 0.1750 | -0.1250 |  |
| riboflavin_b2_mg | 0.6773 | 0.300 | 0.350 | 0.3773 | -0.3273 |  |
| niacin_b3_mg | 11.9710 | 4.200 | 4.900 | 7.7710 | -7.0710 |  |
| vitamin_b6_mg | 0.9178 | 0.360 | 0.420 | 0.5578 | -0.4978 |  |
| folate_ug_dfe | 120.0000 | 120.000 | 140.000 | 0.0000 | 20.0000 | [LB] |
| vitamin_b12_ug | 1.7387 | 0.720 | 0.840 | 1.0187 | -0.8987 |  |
| selenium_ug | 39.5902 | 16.500 | 19.250 | 23.0902 | -20.3402 |  |

## Summary

- **Minimum cost:** $1.0198 per lunch
- **Foods selected:** 10 / 204 available
- **Highest cost item:** Collard Greens, Raw

**Binding lower bounds** (scarce nutrients driving cost up):

- energy_kcal
- calcium_mg
- vitamin_d_ug
- vitamin_e_mg_ate
- folate_ug_dfe

**Binding upper bounds** (limits on cheap food usage):

- total_fat_g
