# Duality Analysis — Children 4 8 Mf

**Solver status:** Optimal  
**Z* (primal):** $0.778860 USD  
**W* (dual):** $0.778860 USD  
**Strong duality Z* = W*:** YES

## Nutrient Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.037226 |
| vitamin_e_mg_ate | min_lb | 2.100 | $0.006266 |
| calcium_mg | min_lb | 300.000 | $0.001205 |
| vitamin_c_mg | min_lb | 7.500 | $0.000748 |
| total_fat_g | range_ub | 23.333 | $0.000694 |
| energy_kcal | range_lb | 550.000 | $0.000643 |
| potassium_mg | min_lb | 690.000 | $0.000181 |
| vitamin_a_ug_rae | min_lb | 120.000 | $0.000064 |
| folate_ug_dfe | min_lb | 60.000 | $0.000010 |

## Group Cap Shadow Prices (Binding Caps)

Shadow price = cost reduction in Z* from relaxing that cap by 1 gram.  
Zero shadow price = cap is not binding for this group.

| Group | Cap (g) | Shadow price (USD/g) |
|-------|--------:|--------------------:|
| cooking_oils | 3.0 | $0.002533 |
| fluid_milk | 150.0 | $0.001547 |

## Complementary Slackness Verification

| Nutrient / Group | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|------------------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 13.493868 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 29.715198 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 2.048019 | 0.000000 | no | no | OK |
| calcium_mg | min_lb | 0.000000 | 0.001205 | YES | YES | OK |
| iron_mg | min_lb | 0.676652 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 134.153311 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 344.682854 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 0.000000 | 0.000181 | YES | YES | OK |
| zinc_mg | min_lb | 1.292517 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | -0.000000 | 0.000064 | YES | YES | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.037226 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | -0.000000 | 0.006266 | YES | YES | OK |
| vitamin_k_ug | min_lb | 44.377218 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | -0.000000 | 0.000748 | YES | YES | OK |
| thiamin_b1_mg | min_lb | 0.382262 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.323938 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 2.913917 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.375253 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | -0.000000 | 0.000010 | YES | YES | OK |
| vitamin_b12_ug | min_lb | 1.454626 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 16.333435 | 0.000000 | no | no | OK |
| sugars_g | max_ub | 5.967903 | 0.000000 | no | no | OK |
| saturated_fat_g | max_ub | 1.974197 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 844.988495 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000643 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 9.323300 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | 0.000000 | 0.000694 | YES | YES | OK |
| fluid_milk | group_cap | 0.000000 | 0.001547 | YES | YES | OK |
| cooking_oils | group_cap | 0.000000 | 0.002533 | YES | YES | OK |
| grain_products | group_cap | 47.042751 | 0.000000 | no | no | OK |
| leafy_veg | group_cap | 66.992866 | 0.000000 | no | no | OK |
| protein_foods | group_cap | 76.830610 | 0.000000 | no | no | OK |
| fruits | group_cap | 112.318689 | 0.000000 | no | no | OK |
