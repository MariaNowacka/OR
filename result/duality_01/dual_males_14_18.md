# Duality Analysis — Males 14 18

**Solver status:** Optimal  
**Z* (primal):** $0.927501 USD  
**W* (dual):** $0.927501 USD  
**Strong duality Z* = W*:** YES

## Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.062071 |
| dietary_fiber_g | min_lb | 11.400 | $0.018164 |
| vitamin_e_mg_ate | min_lb | 4.500 | $0.007420 |
| sugars_g | max_ub | 20.000 | $0.005981 |
| vitamin_c_mg | min_lb | 22.500 | $0.002726 |
| total_fat_g | range_ub | 31.111 | $0.001360 |
| folate_ug_dfe | min_lb | 120.000 | $0.000677 |
| energy_kcal | range_lb | 750.000 | $0.000410 |
| calcium_mg | min_lb | 390.000 | $0.000241 |
| vitamin_a_ug_rae | min_lb | 270.000 | $0.000116 |

## Complementary Slackness Verification

| Nutrient | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|----------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 5.327493 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 62.649489 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 0.000000 | 0.018164 | YES | YES | OK |
| calcium_mg | min_lb | 0.000000 | 0.000241 | YES | YES | OK |
| iron_mg | min_lb | 3.749210 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 71.245386 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 202.243590 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 47.727147 | 0.000000 | no | no | OK |
| zinc_mg | min_lb | 0.242628 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 0.000000 | 0.000116 | YES | YES | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.062071 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | 0.000000 | 0.007420 | YES | YES | OK |
| vitamin_k_ug | min_lb | 21.989787 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | 0.000000 | 0.002726 | YES | YES | OK |
| thiamin_b1_mg | min_lb | 0.505048 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.676891 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 2.768297 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.614139 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | 0.000000 | 0.000677 | YES | YES | OK |
| vitamin_b12_ug | min_lb | 2.407429 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 9.030145 | 0.000000 | no | no | OK |
| sugars_g | max_ub | -0.000000 | 0.005981 | YES | YES | OK |
| saturated_fat_g | max_ub | 2.061980 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 999.093479 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000410 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 5.101100 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | 0.000000 | 0.001360 | YES | YES | OK |
