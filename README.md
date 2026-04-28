# Operations Research — Minimum-Cost School Lunch Optimisation (U.S.)

Linear programming project to minimise the cost of a nutritionally compliant school lunch
for U.S. school-age children (ages 4–18), across five age-sex groups, using 2024 official
U.S. dietary requirements and retail food price data.

### Resources

* [USDA FoodData Central — SR Legacy / Foundation Foods](https://fdc.nal.usda.gov)

* [BLS CPI Average Price Series](https://data.bls.gov)

* [USDA ERS Meat Price Spreads](https://www.ers.usda.gov/data-products/meat-price-spreads)

* [USDA ERS Fruit and Vegetable Prices](https://www.ers.usda.gov/topics/food-markets-prices)

* [National Academies DRI Tables (NCBI Bookshelf)](https://www.ncbi.nlm.nih.gov/books/NBK56068/)

* [USDA NSLP Meal Pattern 2024 (Federal Register)](https://www.federalregister.gov/documents/2024/04/25/2024-08098)

* [Dietary Guidelines for Americans 2020–2025](https://www.dietaryguidelines.gov)

python version = 3.12.9

required libraries to install: `requirements.txt` (based on arm64-osx)

**Before you run**

Place all data files in your local `data/` folder before running any notebook:

* `food_nutrition_200.xlsx` — 205 foods × 29 nutrients per 100 g (USDA FoodData Central)

* `food_prices_200.xlsx` — 205 foods × price per gram, BLS CPI 2024 annual average

* `dri_lunch_lb.csv` — per-meal DRI lower bounds (30 % of daily RDA/AI) per age-sex group

* `dri_lunch_ub.csv` — per-meal DRI upper bounds (35 % of daily DRI / NSLP caps) per age-sex group

Update `PATH_NUTRITION`, `PATH_PRICES`, `PATH_REQ_LB`, `PATH_REQ_UB` and `SAVE_PATH`
at the top of each notebook to match your local directory structure.

If your machine is Apple Silicon (arm64 macOS), all libraries install normally via pip
in a standard venv — no special flags required for this project.

# Experiments

Experiments follow the LP pipeline sequentially. Each notebook is self-contained
and can be run independently, as long as the four data files above are present.

Results are saved as Markdown files in `result/` subfolders for each step.

## Step 00 Linear Programming

Formulates and solves the cost-minimisation LP for five age-sex groups
(children 4–8, males 9–13, females 9–13, males 14–18, females 14–18).

**Objective function**: minimise total lunch cost $Z = \sum_i c_i x_i$
where $c_i$ is price per gram and $x_i$ is grams of food $i$ selected.

**Constraints**: 21 nutritional lower bounds (RDA/AI), 3 upper bounds (NSLP/DGA limits),
2 range constraints (energy window + fat AMDR), and a 200 g per-food portion cap.

Solver: `scipy.optimize.linprog` with HiGHS backend.

### Code

* [Step 00 Linear Programming](https://github.com/MariaNowacka/OR/blob/main/code/00_Linear_Programming.ipynb)

### Results

Optimal lunch menu, nutritional achievement vs. DRI bounds, and binding constraint
analysis for each age-sex group.

* [Results — Children 4–8](https://github.com/MariaNowacka/OR/blob/main/result/linprog_02/results_children_4_8_MF.md)

* [Results — Males 9–13](https://github.com/MariaNowacka/OR/blob/main/result/linprog_02/results_males_9_13.md)

* [Results — Females 9–13](https://github.com/MariaNowacka/OR/blob/main/result/linprog_02/results_females_9_13.md)

* [Results — Males 14–18](https://github.com/MariaNowacka/OR/blob/main/result/linprog_02/results_males_14_18.md)

* [Results — Females 14–18](https://github.com/MariaNowacka/OR/blob/main/result/linprog_02/results_females_14_18.md)

Minimum costs: children 4–8 = $0.69 · males 9–13 = $0.79 · females 9–13 = $0.77 · males 14–18 = $0.93 · females 14–18 = $0.87 (per lunch, 2024 prices)

Consistently binding lower bounds across all groups: `energy_kcal`, `calcium_mg`, `vitamin_d_ug`, `vitamin_a_ug_rae`, `folate_ug_dfe`, `vitamin_c_mg`

Consistently binding upper bounds: `total_fat_g` (AMDR 35 % ceiling), `sugars_g` (DGA 10 % limit)

## Step 01 Sensitivity Analysis

Investigates how changes in the objective coefficients ($\Delta c$) and constraint
right-hand sides ($\Delta b$) affect the optimal solution.

**Range of optimality** ($\Delta c$): how much can food prices change before the
optimal menu changes? Identifies which food prices the solution is most sensitive to.

**Range of feasibility** ($\Delta b$): how much can each DRI bound change before
the current basis is no longer feasible? Quantifies the cost impact of policy changes
to nutritional standards.

### Code

* [Step 01 Sensitivity Analysis](https://github.com/MariaNowacka/OR/blob/main/code/01_Sensitivity_Analysis.ipynb)

### Results

Ranging tables for objective coefficients and RHS constraints per age-sex group.

* [Sensitivity — Children 4–8](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/sensitivity/sensitivity_children_4_8_MF.md)

* [Sensitivity — Males 9–13](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/sensitivity/sensitivity_males_9_13.md)

* [Sensitivity — Females 9–13](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/sensitivity/sensitivity_females_9_13.md)

* [Sensitivity — Males 14–18](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/sensitivity/sensitivity_males_14_18.md)

* [Sensitivity — Females 14–18](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/sensitivity/sensitivity_females_14_18.md)

## Step 02 Duality

Derives and analyses the dual problem associated with the primal cost-minimisation LP.

**Dual objective**: $W^* = \mathbf{b}_{ub}^\top \boldsymbol{\mu} + x_{ub} \cdot \mathbf{1}^\top \boldsymbol{\lambda}_{ub}$

**Shadow prices** ($\mu_k$): marginal cost of tightening each nutritional constraint by
one unit. A shadow price of $s$ on nutrient $j$ means: requiring 1 more unit of nutrient
$j$ per lunch increases the minimum cost by $s$ USD.

**Strong duality verified**: $Z^* = W^*$ for all five groups (numerical gap < 1e-4).

**Complementary slackness verified**: binding constraints have nonzero shadow prices;
non-binding constraints have shadow price = 0.

Dual variables sourced from `res.ineqlin.marginals` and `res.upper.marginals`
(scipy HiGHS).

### Code

* [Step 02 Duality](https://github.com/MariaNowacka/OR/blob/main/code/02_Duality.ipynb)

### Results

Shadow price tables, strong duality verification ($Z^* = W^*$), and complementary
slackness check for each age-sex group.

* [Dual — Children 4–8](https://github.com/MariaNowacka/OR/blob/main/result/duality_01/dual_children_4_8_MF.md)

* [Dual — Males 9–13](https://github.com/MariaNowacka/OR/blob/main/result/duality_01/dual_males_9_13.md)

* [Dual — Females 9–13](https://github.com/MariaNowacka/OR/blob/main/result/duality_01/dual_females_9_13.md)

* [Dual — Males 14–18](https://github.com/MariaNowacka/OR/blob/main/result/duality_01/dual_males_14_18.md)

* [Dual — Females 14–18](https://github.com/MariaNowacka/OR/blob/main/result/duality_01/dual_females_14_18.md)

Most expensive constraint to tighten across all groups: `vitamin_d_ug`
(shadow price ≈ $0.062 per µg increase in requirement for males 14–18)

## Step 03 Upper Bound Technique

Applies tighter, food-category-specific portion caps to address the liquid-dominance
problem identified in Step 00, where the unconstrained LP selected unrealistically
large quantities of fluid milk and vegetable oil.

**Motivation**: the Step 00 solution (e.g. 270 g milk + 90 g dry cornmeal) is
nutritionally valid but not a realistic school lunch menu. The Upper Bound Technique
is the formal mechanism for handling bounded variables
efficiently within simplex without expanding the constraint matrix.

**Category-specific caps applied**:

* Fluid milk: ≤ 240 g (one standard 8 fl oz school carton)

* Cooking oils: ≤ 10 g (cooking use only, not a served dish)

* Dry grains / raw ingredients: ≤ 80 g (cooked equivalent portion)

* All other foods: ≤ 200 g

The tighter bounds force the LP to source nutrients from a broader range of foods,
producing a more diverse and realistic menu at an increased but bounded cost.

### Code

* [Step 03 Upper Bound Technique](https://github.com/MariaNowacka/OR/blob/main/code/03_Upper_Bound_Technique.ipynb)

### Results

Revised optimal menus under category-specific bounds, cost comparison against
Step 00 baseline, and analysis of which foods replace milk and cornmeal
as binding-constraint drivers.

* [Upper Bound — Children 4–8](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/upper_bound/ub_children_4_8_MF.md)

* [Upper Bound — Males 9–13](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/upper_bound/ub_males_9_13.md)

* [Upper Bound — Females 9–13](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/upper_bound/ub_females_9_13.md)

* [Upper Bound — Males 14–18](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/upper_bound/ub_males_14_18.md)

* [Upper Bound — Females 14–18](https://github.com/YOUR_USERNAME/YOUR_REPO/blob/main/result/upper_bound/ub_females_14_18.md)
