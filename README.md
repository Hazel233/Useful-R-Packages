
<!-- README.md is generated from README.Rmd. Please edit that file -->

# funfurther

<!-- badges: start -->

<!-- badges: end -->

The goal of funfurther is to add some new features to existing
`strsplit` function.

## Installation

You can install the released version of funfurther from
[CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("devtools")
```

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("Hazel233/Useful-R-Packages")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(funfurther)
#> 
#> Attaching package: 'funfurther'
#> The following object is masked from 'package:base':
#> 
#>     strsplit
x <- c("3D/MON&SUN")
strsplit(x, "", type = "before")
#> [[1]]
#>  [1] "3" "D" "/" "M" "O" "N" "&" "S" "U" "N"
```

## Assignment2-STAT545B

My first R Package repository on GitHub starting from STAT545B. The
following parts are some explanation for this assignment\!

### E1.1 The explaination of the development

`library(devtools)` is used to prepare for the tools. Then,
`create_package("~/Desktop/funfurther")` and `use_git()` are introduced
for create folder in user’s desktop and prepare for git operation
seperately. `use_r("strsplit")` can save the function in a `.R` file.
Finally use `load_all()` to make the function available for
experimentation. To be sure that all the moving parts of the foofactors
package still work, apply `check()` to do this. And use
`use_mit_license("Hazel Hao")` to set license for one’s work.

### E1.2 Tests

`usethis` and `testthat` are used especially to test those new
functions.

### E1.3 Documentation of the R package

1.  `document()` is used to update my documentation. The only object is
    set to be exported for use.
2.  Other tasks have been done and can be found in corresponding files.
