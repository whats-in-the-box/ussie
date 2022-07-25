
<!-- README.md is generated from README.Rmd. Please edit that file -->

# ussie

<!-- badges: start -->

[![R-CMD-check](https://github.com/whats-in-the-box/ussie/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/whats-in-the-box/ussie/actions/workflows/R-CMD-check.yaml)
[![test-coverage](https://github.com/whats-in-the-box/ussie/actions/workflows/test-coverage.yaml/badge.svg)](https://github.com/whats-in-the-box/ussie/actions/workflows/test-coverage.yaml)
<!-- badges: end -->

The goal of ussie is to help you to work with European football league
data supplied by the **`engsoccerdata`** package (Curley 2016).

## Installation

You can install the development version of ussie from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("whats-in-the-box/ussie")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(ussie)
## basic example code
uss_make_matches(engsoccerdata::spain, "Spain")
#> # A tibble: 23,915 x 8
#>    country tier  season date       home               visitor    goals~1 goals~2
#>    <chr>   <fct>  <int> <date>     <chr>              <chr>        <int>   <int>
#>  1 Spain   1       1928 1929-02-10 Arenas de Getxo    Atletico ~       2       3
#>  2 Spain   1       1928 1929-02-10 Espanyol Barcelona Real Union       3       2
#>  3 Spain   1       1928 1929-02-10 Real Madrid        CE Europa        5       0
#>  4 Spain   1       1928 1929-02-10 Real Sociedad      Athletic ~       1       1
#>  5 Spain   1       1928 1929-02-12 Racing Santander   FC Barcel~       0       2
#>  6 Spain   1       1928 1929-02-17 FC Barcelona       Real Madr~       1       2
#>  7 Spain   1       1928 1929-02-17 Athletic Bilbao    Espanyol ~       9       0
#>  8 Spain   1       1928 1929-02-17 Atletico Madrid    Real Soci~       0       3
#>  9 Spain   1       1928 1929-02-17 Real Union         Racing Sa~       3       1
#> 10 Spain   1       1928 1929-02-17 CE Europa          Arenas de~       5       2
#> # ... with 23,905 more rows, and abbreviated variable names 1: goals_home,
#> #   2: goals_visitor
#> # i Use `print(n = ...)` to see more rows
```
