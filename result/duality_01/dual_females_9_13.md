# Duality Analysis — Females 9 13

**Solver status:** Optimal  
**Z* (primal):** $0.773432 USD  
**W* (dual):** $0.773432 USD  
**Strong duality Z* = W*:** YES

## Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.060767 |
| dietary_fiber_g | min_lb | 7.800 | $0.013972 |
| sugars_g | max_ub | 16.250 | $0.010637 |
| vitamin_c_mg | min_lb | 13.500 | $0.002997 |
| folate_ug_dfe | min_lb | 90.000 | $0.000852 |
| total_fat_g | range_ub | 25.278 | $0.000831 |
| energy_kcal | range_lb | 600.000 | $0.000493 |
| calcium_mg | min_lb | 390.000 | $0.000406 |
| vitamin_a_ug_rae | min_lb | 180.000 | $0.000105 |

## Complementary Slackness Verification

| Nutrient | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|----------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 7.850739 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 39.248881 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | -0.000000 | 0.013972 | YES | YES | OK |
| calcium_mg | min_lb | 0.000000 | 0.000406 | YES | YES | OK |
| iron_mg | min_lb | 1.909504 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 73.340920 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 106.272812 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 86.368554 | 0.000000 | no | no | OK |
| zinc_mg | min_lb | 0.336391 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 0.000000 | 0.000105 | YES | YES | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.060767 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | 0.022824 | 0.000000 | no | no | OK |
| vitamin_k_ug | min_lb | 70.368560 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | 0.000000 | 0.002997 | YES | YES | OK |
| thiamin_b1_mg | min_lb | 0.357294 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.597084 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 1.893139 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.498566 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | 0.000000 | 0.000852 | YES | YES | OK |
| vitamin_b12_ug | min_lb | 1.418515 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 10.096010 | 0.000000 | no | no | OK |
| sugars_g | max_ub | 0.000000 | 0.010637 | YES | YES | OK |
| saturated_fat_g | max_ub | 0.908062 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 974.982754 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | -0.000000 | 0.000493 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 9.287800 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | 0.000000 | 0.000831 | YES | YES | OK |
