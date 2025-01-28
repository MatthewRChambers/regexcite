
<!-- README.md is generated from README.Rmd. Please edit that file -->

# regexcite

<!-- badges: start -->
<!-- badges: end -->

The goal of regexcite is to make regular expressions more exciting! It
provides convinience functions to make some common tasks with string
manipulation and regular expressions a bit easier.

## Installation

You can install the development version of regexcite from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("MatthewRChambers/regexcite")
```

## Usage

This is a basic example which shows you how to solve a common problem:

``` r
library(regexcite)

x = "alfa,bravo,charlie,delta"
str_split_one(x, pattern = ",")
#> [1] "alfa"    "bravo"   "charlie" "delta"
str_split_one(x, pattern = ",", n = 2)
#> [1] "alfa"                "bravo,charlie,delta"

y = "192.168.0.1"
str_split_one(y, pattern = ".", n = 2)
#> [1] ""           "92.168.0.1"
```
