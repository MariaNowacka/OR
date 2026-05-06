# Duality Analysis — Females 9 13

**Solver status:** Optimal  
**Z* (primal):** $0.941642 USD  
**W* (dual):** $0.941642 USD  
**Strong duality Z* = W*:** YES

## Nutrient Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.035600 |
| vitamin_e_mg_ate | min_lb | 3.300 | $0.005292 |
| calcium_mg | min_lb | 390.000 | $0.001345 |
| total_fat_g | range_ub | 25.278 | $0.001033 |
| energy_kcal | range_lb | 600.000 | $0.000691 |
| potassium_mg | min_lb | 690.000 | $0.000117 |
| folate_ug_dfe | min_lb | 90.000 | $0.000074 |
| vitamin_a_ug_rae | min_lb | 180.000 | $0.000065 |

## Group Cap Shadow Prices (Binding Caps)

Shadow price = cost reduction in Z* from relaxing that cap by 1 gram.  
Zero shadow price = cap is not binding for this group.

| Group | Cap (g) | Shadow price (USD/g) |
|-------|--------:|--------------------:|
| cooking_oils | 3.0 | $0.002450 |
| fluid_milk | 150.0 | $0.001605 |

## Complementary Slackness Verification

| Nutrient / Group | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|------------------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 10.131874 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 36.818306 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 1.317926 | 0.000000 | no | no | OK |
| calcium_mg | min_lb | 0.000000 | 0.001345 | YES | YES | OK |
| iron_mg | min_lb | 1.347198 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 91.339469 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 116.922667 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 0.000000 | 0.000117 | YES | YES | OK |
| zinc_mg | min_lb | 0.475106 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 0.000000 | 0.000065 | YES | YES | OK |
| vitamin_d_ug | min_lb | -0.000000 | 0.035600 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | 0.000000 | 0.005292 | YES | YES | OK |
| vitamin_k_ug | min_lb | 167.538568 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | 1.131656 | 0.000000 | no | no | OK |
| thiamin_b1_mg | min_lb | 0.216616 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.270896 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 1.908475 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.290936 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | 0.000000 | 0.000074 | YES | YES | OK |
| vitamin_b12_ug | min_lb | 1.064153 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 12.345893 | 0.000000 | no | no | OK |
| sugars_g | max_ub | 8.035400 | 0.000000 | no | no | OK |
| saturated_fat_g | max_ub | 1.272848 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 895.286011 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000691 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 9.287800 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | 0.000000 | 0.001033 | YES | YES | OK |
| fluid_milk | group_cap | 0.000000 | 0.001605 | YES | YES | OK |
| cooking_oils | group_cap | 0.000000 | 0.002450 | YES | YES | OK |
| grain_products | group_cap | 35.659225 | 0.000000 | no | no | OK |
| leafy_veg | group_cap | 38.626851 | 0.000000 | no | no | OK |
| protein_foods | group_cap | 78.232918 | 0.000000 | no | no | OK |
| fruits | group_cap | 120.000000 | 0.000000 | no | no | OK |
