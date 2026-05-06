# Duality Analysis — Males 9 13

**Solver status:** Optimal  
**Z* (primal):** $0.948933 USD  
**W* (dual):** $0.948933 USD  
**Strong duality Z* = W*:** YES

## Nutrient Shadow Prices (Binding Constraints)

Shadow price = cost increase in Z* from tightening that constraint by 1 unit.  
Zero shadow price = non-binding constraint (complementary slackness).

| Nutrient | Constraint type | RHS | Shadow price (USD/unit) |
|----------|----------------|----:|------------------------:|
| vitamin_d_ug | min_lb | 4.500 | $0.035438 |
| vitamin_e_mg_ate | min_lb | 3.300 | $0.005340 |
| calcium_mg | min_lb | 390.000 | $0.001345 |
| total_fat_g | range_ub | 25.278 | $0.001017 |
| energy_kcal | range_lb | 600.000 | $0.000689 |
| vitamin_c_mg | min_lb | 13.500 | $0.000199 |
| potassium_mg | min_lb | 750.000 | $0.000125 |
| vitamin_a_ug_rae | min_lb | 180.000 | $0.000068 |

## Group Cap Shadow Prices (Binding Caps)

Shadow price = cost reduction in Z* from relaxing that cap by 1 gram.  
Zero shadow price = cap is not binding for this group.

| Group | Cap (g) | Shadow price (USD/g) |
|-------|--------:|--------------------:|
| cooking_oils | 3.0 | $0.002461 |
| fluid_milk | 150.0 | $0.001613 |

## Complementary Slackness Verification

| Nutrient / Group | Type | Slack | Shadow price | Binding | SP != 0 | CS holds |
|------------------|------|------:|-------------:|:-------:|:-------:|:--------:|
| protein_g | min_lb | 10.961172 | 0.000000 | no | no | OK |
| carbohydrates_g | min_lb | 36.693015 | 0.000000 | no | no | OK |
| dietary_fiber_g | min_lb | 2.193325 | 0.000000 | no | no | OK |
| calcium_mg | min_lb | 0.000000 | 0.001345 | YES | YES | OK |
| iron_mg | min_lb | 1.787471 | 0.000000 | no | no | OK |
| magnesium_mg | min_lb | 124.564249 | 0.000000 | no | no | OK |
| phosphorus_mg | min_lb | 157.557892 | 0.000000 | no | no | OK |
| potassium_mg | min_lb | 0.000000 | 0.000125 | YES | YES | OK |
| zinc_mg | min_lb | 0.737396 | 0.000000 | no | no | OK |
| vitamin_a_ug_rae | min_lb | 0.000000 | 0.000068 | YES | YES | OK |
| vitamin_d_ug | min_lb | 0.000000 | 0.035438 | YES | YES | OK |
| vitamin_e_mg_ate | min_lb | -0.000000 | 0.005340 | YES | YES | OK |
| vitamin_k_ug | min_lb | 152.146603 | 0.000000 | no | no | OK |
| vitamin_c_mg | min_lb | 0.000000 | 0.000199 | YES | YES | OK |
| thiamin_b1_mg | min_lb | 0.364057 | 0.000000 | no | no | OK |
| riboflavin_b2_mg | min_lb | 0.268566 | 0.000000 | no | no | OK |
| niacin_b3_mg | min_lb | 2.178053 | 0.000000 | no | no | OK |
| vitamin_b6_mg | min_lb | 0.319039 | 0.000000 | no | no | OK |
| folate_ug_dfe | min_lb | 3.444206 | 0.000000 | no | no | OK |
| vitamin_b12_ug | min_lb | 1.248082 | 0.000000 | no | no | OK |
| selenium_ug | min_lb | 14.180839 | 0.000000 | no | no | OK |
| sugars_g | max_ub | 8.156511 | 0.000000 | no | no | OK |
| saturated_fat_g | max_ub | 2.007101 | 0.000000 | no | no | OK |
| sodium_mg | max_ub | 934.482031 | 0.000000 | no | no | OK |
| energy_kcal | range_lb | 0.000000 | 0.000689 | YES | YES | OK |
| energy_kcal | range_ub | 100.000000 | 0.000000 | no | no | OK |
| total_fat_g | range_lb | 7.277800 | 0.000000 | no | no | OK |
| total_fat_g | range_ub | -0.000000 | 0.001017 | YES | YES | OK |
| fluid_milk | group_cap | 0.000000 | 0.001613 | YES | YES | OK |
| cooking_oils | group_cap | 0.000000 | 0.002461 | YES | YES | OK |
| grain_products | group_cap | 39.051905 | 0.000000 | no | no | OK |
| leafy_veg | group_cap | 41.990228 | 0.000000 | no | no | OK |
| protein_foods | group_cap | 77.056494 | 0.000000 | no | no | OK |
| fruits | group_cap | 120.000000 | 0.000000 | no | no | OK |
