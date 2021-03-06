# ompr 0.7.0.9002

* Removed `dplyr` dependency
* Added `MILPModel`, a new, vectorized backend for mixed integer linear programs that can handle very large models. It will eventually replace `MIPModel`.
* Added two functions (`get_column_duals`, `get_row_duals`) to extract the dual (column and row) values from an LP.
* The minimum supported R version is now `3.2.0`
* `get_solution` now always return a solution, even if the solution status is not optimal.
* `get_solution` has a third argument `type` with permitted values being "primal" and "dual" to return the respective column primal or dual values.

# ompr 0.7.0

## Breaking changes

* `ompr` now uses sparse constraint matrices. `extract_constraints` now returns a sparse matrix and `objective_function` returns a sparse vector.
* The minimum supported R version is now `3.3.0`
* Fixed an issue with `Rcpp`. The minimum `Rcpp` version is now `0.12.12`

## Minor changes

* New progress bar based on the `progress` package.

# ompr 0.6.0

* First version on CRAN


