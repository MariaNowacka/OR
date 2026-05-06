# Duality Analysis — Males 14 18

**Solver status:** Optimal  
**Z* (primal):** $1.085043 USD  
**W* (dual):** $1.085043 USD  
**Strong duality Z* = W*:** YES

## Nutrient Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.037145 |
| vitamin_e_mg_ate | min_lb | 4.500 | $0.006328 |
| calcium_mg | min_lb | 390.000 | $0.001209 |
| vitamin_c_mg | min_lb | 22.500 | $0.000756 |
| total_fat_g | range_ub | 31.111 | $0.000704 |
| energy_kcal | range_lb | 750.000 | $0.000644 |
| potassium_mg | min_lb | 900.000 | $0.000180 |
| vitamin_a_ug_rae | min_lb | 270.000 | $0.000064 |

## Group Cap Shadow Prices (Binding Caps)

Shadow price = cost reduction in Z* from relaxing that cap by 1 gram.  
Zero shadow price = cap is not binding for this group.

| Group | Cap (g) | Shadow price (USD/g) |
|-------|--------:|--------------------:|
| cooking_oils | 3.0 | $0.002542 |
| fluid_milk | 150.0 | $0.001550 |

## Complementary Slackness Verification

| Nutrient / Group | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|------------------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 7.475911 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 60.268637 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 1.898891 | 0.000000 | no | no | OK |
| calcium_mg | min_lb | 0.000000 | 0.001209 | YES | YES | OK |
| iron_mg | min_lb | 1.771454 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 100.514488 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 226.613413 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 0.000000 | 0.000180 | YES | YES | OK |
| zinc_mg | min_lb | 0.322509 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 0.000000 | 0.000064 | YES | YES | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.037145 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | 0.000000 | 0.006328 | YES | YES | OK |
| vitamin_k_ug | min_lb | 213.198085 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | 0.000000 | 0.000756 | YES | YES | OK |
| thiamin_b1_mg | min_lb | 0.326111 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.219405 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 2.163705 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.377309 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | 3.391479 | 0.000000 | no | no | OK |
| vitamin_b12_ug | min_lb | 0.806118 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 13.369036 | 0.000000 | no | no | OK |
| sugars_g | max_ub | 10.043972 | 0.000000 | no | no | OK |
| saturated_fat_g | max_ub | 3.011982 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 949.019899 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000644 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 5.101100 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | 0.000000 | 0.000704 | YES | YES | OK |
| fluid_milk | group_cap | 0.000000 | 0.001550 | YES | YES | OK |
| cooking_oils | group_cap | 0.000000 | 0.002542 | YES | YES | OK |
| grain_products | group_cap | 11.915334 | 0.000000 | no | no | OK |
| leafy_veg | group_cap | 27.486206 | 0.000000 | no | no | OK |
| protein_foods | group_cap | 78.604048 | 0.000000 | no | no | OK |
| fruits | group_cap | 113.143097 | 0.000000 | no | no | OK |
