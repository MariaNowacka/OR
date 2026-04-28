# Duality Analysis — Children 4 8 Mf

**Solver status:** Optimal  
**Z* (primal):** $0.687245 USD  
**W* (dual):** $0.687245 USD  
**Strong duality Z* = W*:** YES

## Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.067207 |
| dietary_fiber_g | min_lb | 7.500 | $0.017972 |
| sugars_g | max_ub | 15.000 | $0.005638 |
| vitamin_c_mg | min_lb | 7.500 | $0.002607 |
| energy_kcal | range_lb | 550.000 | $0.000431 |
| folate_ug_dfe | min_lb | 60.000 | $0.000405 |
| total_fat_g | range_ub | 23.333 | $0.000303 |
| vitamin_k_ug | min_lb | 16.500 | $0.000258 |
| calcium_mg | min_lb | 300.000 | $0.000138 |
| vitamin_a_ug_rae | min_lb | 120.000 | $0.000128 |

## Complementary Slackness Verification

| Nutrient | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|----------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 11.624112 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 31.812319 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 0.000000 | 0.017972 | YES | YES | OK |
| calcium_mg | min_lb | 0.000000 | 0.000138 | YES | YES | OK |
| iron_mg | min_lb | 1.027140 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 105.635211 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 301.904550 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 10.979079 | 0.000000 | no | no | OK |
| zinc_mg | min_lb | 0.979742 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 0.000000 | 0.000128 | YES | YES | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.067207 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | 0.777465 | 0.000000 | no | no | OK |
| vitamin_k_ug | min_lb | -0.000000 | 0.000258 | YES | YES | OK |
| vitamin_c_mg | min_lb | 0.000000 | 0.002607 | YES | YES | OK |
| thiamin_b1_mg | min_lb | 0.408532 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.506472 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 3.169379 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.475286 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | -0.000000 | 0.000405 | YES | YES | OK |
| vitamin_b12_ug | min_lb | 1.409525 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 13.311091 | 0.000000 | no | no | OK |
| sugars_g | max_ub | 0.000000 | 0.005638 | YES | YES | OK |
| saturated_fat_g | max_ub | 1.750405 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 872.806027 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000431 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 9.323300 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | -0.000000 | 0.000303 | YES | YES | OK |
