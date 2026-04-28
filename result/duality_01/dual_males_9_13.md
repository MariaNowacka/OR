# Duality Analysis — Males 9 13

**Solver status:** Optimal  
**Z* (primal):** $0.796206 USD  
**W* (dual):** $0.796206 USD  
**Strong duality Z* = W*:** YES

## Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.061365 |
| dietary_fiber_g | min_lb | 9.300 | $0.015234 |
| sugars_g | max_ub | 16.250 | $0.009829 |
| vitamin_e_mg_ate | min_lb | 3.300 | $0.003391 |
| vitamin_c_mg | min_lb | 13.500 | $0.002912 |
| total_fat_g | range_ub | 25.278 | $0.001189 |
| folate_ug_dfe | min_lb | 90.000 | $0.000817 |
| energy_kcal | range_lb | 600.000 | $0.000468 |
| calcium_mg | min_lb | 390.000 | $0.000385 |
| vitamin_a_ug_rae | min_lb | 180.000 | $0.000107 |

## Complementary Slackness Verification

| Nutrient | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|----------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 8.210620 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 39.235973 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 0.000000 | 0.015234 | YES | YES | OK |
| calcium_mg | min_lb | 0.000000 | 0.000385 | YES | YES | OK |
| iron_mg | min_lb | 2.422773 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 92.470801 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 130.729725 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 54.433928 | 0.000000 | no | no | OK |
| zinc_mg | min_lb | 0.505939 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 0.000000 | 0.000107 | YES | YES | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.061365 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | -0.000000 | 0.003391 | YES | YES | OK |
| vitamin_k_ug | min_lb | 31.842808 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | 0.000000 | 0.002912 | YES | YES | OK |
| thiamin_b1_mg | min_lb | 0.475464 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.622780 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 2.186038 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.538622 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | 0.000000 | 0.000817 | YES | YES | OK |
| vitamin_b12_ug | min_lb | 1.585216 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 11.078160 | 0.000000 | no | no | OK |
| sugars_g | max_ub | 0.000000 | 0.009829 | YES | YES | OK |
| saturated_fat_g | max_ub | 1.170093 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 963.768772 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000468 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 7.277800 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | 0.000000 | 0.001189 | YES | YES | OK |
