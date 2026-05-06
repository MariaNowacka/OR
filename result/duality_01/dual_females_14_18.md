# Duality Analysis — Females 14 18

**Solver status:** Optimal  
**Z* (primal):** $1.060968 USD  
**W* (dual):** $1.060968 USD  
**Strong duality Z* = W*:** YES

## Nutrient Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.037794 |
| vitamin_e_mg_ate | min_lb | 4.500 | $0.004393 |
| total_fat_g | range_ub | 31.111 | $0.001722 |
| calcium_mg | min_lb | 390.000 | $0.001362 |
| energy_kcal | range_lb | 750.000 | $0.000773 |
| folate_ug_dfe | min_lb | 120.000 | $0.000362 |

## Group Cap Shadow Prices (Binding Caps)

Shadow price = cost reduction in Z* from relaxing that cap by 1 gram.  
Zero shadow price = cap is not binding for this group.

| Group | Cap (g) | Shadow price (USD/g) |
|-------|--------:|--------------------:|
| cooking_oils | 3.0 | $0.002338 |
| fluid_milk | 150.0 | $0.001486 |

## Complementary Slackness Verification

| Nutrient / Group | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|------------------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 7.218304 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 61.396366 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 3.005602 | 0.000000 | no | no | OK |
| calcium_mg | min_lb | 0.000000 | 0.001362 | YES | YES | OK |
| iron_mg | min_lb | 0.162576 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 79.724541 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 134.085561 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 85.619916 | 0.000000 | no | no | OK |
| zinc_mg | min_lb | 0.459015 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 17.910624 | 0.000000 | no | no | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.037794 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | -0.000000 | 0.004393 | YES | YES | OK |
| vitamin_k_ug | min_lb | 257.100281 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | 2.496125 | 0.000000 | no | no | OK |
| thiamin_b1_mg | min_lb | 0.230893 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.295228 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 2.354100 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.342227 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | 0.000000 | 0.000362 | YES | YES | OK |
| vitamin_b12_ug | min_lb | 0.765993 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 8.757361 | 0.000000 | no | no | OK |
| sugars_g | max_ub | 11.608356 | 0.000000 | no | no | OK |
| saturated_fat_g | max_ub | 2.631430 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 902.678387 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000773 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 11.101100 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | 0.000000 | 0.001722 | YES | YES | OK |
| fluid_milk | group_cap | 0.000000 | 0.001486 | YES | YES | OK |
| cooking_oils | group_cap | 0.000000 | 0.002338 | YES | YES | OK |
| grain_products | group_cap | 3.108081 | 0.000000 | no | no | OK |
| leafy_veg | group_cap | 17.688031 | 0.000000 | no | no | OK |
| protein_foods | group_cap | 79.948840 | 0.000000 | no | no | OK |
| fruits | group_cap | 120.000000 | 0.000000 | no | no | OK |
