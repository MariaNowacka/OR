# Duality Analysis — Females 14 18

**Solver status:** Optimal  
**Z* (primal):** $0.875591 USD  
**W* (dual):** $0.875591 USD  
**Strong duality Z* = W*:** YES

## Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.044148 |
| sugars_g | max_ub | 20.000 | $0.008367 |
| total_fat_g | range_ub | 31.111 | $0.003418 |
| vitamin_c_mg | min_lb | 19.500 | $0.003215 |
| folate_ug_dfe | min_lb | 120.000 | $0.001164 |
| energy_kcal | range_lb | 750.000 | $0.000774 |
| vitamin_e_mg_ate | min_lb | 4.500 | $0.000600 |
| calcium_mg | min_lb | 390.000 | $0.000395 |
| vitamin_a_ug_rae | min_lb | 210.000 | $0.000085 |

## Complementary Slackness Verification

| Nutrient | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|----------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 6.085381 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 63.073989 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 1.345978 | 0.000000 | no | no | OK |
| calcium_mg | min_lb | 0.000000 | 0.000395 | YES | YES | OK |
| iron_mg | min_lb | 2.324320 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 58.025957 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 166.267614 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 213.609927 | 0.000000 | no | no | OK |
| zinc_mg | min_lb | 0.630130 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 0.000000 | 0.000085 | YES | YES | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.044148 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | -0.000000 | 0.000600 | YES | YES | OK |
| vitamin_k_ug | min_lb | 54.077269 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | -0.000000 | 0.003215 | YES | YES | OK |
| thiamin_b1_mg | min_lb | 0.426065 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.730375 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 3.039576 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.626147 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | -0.000000 | 0.001164 | YES | YES | OK |
| vitamin_b12_ug | min_lb | 1.303752 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 7.375854 | 0.000000 | no | no | OK |
| sugars_g | max_ub | -0.000000 | 0.008367 | YES | YES | OK |
| saturated_fat_g | max_ub | 1.522354 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 1009.158773 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000774 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 11.101100 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | 0.000000 | 0.003418 | YES | YES | OK |
