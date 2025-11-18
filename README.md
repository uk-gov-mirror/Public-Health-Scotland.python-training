# python-training
This is an interactive, online introduction to python training for employees 
in Public Health Scotland.

The R packages required to render this course are `learnr`, `reticulate`, 
and `gradethis`. 

- `learnr` and `reticulate` can be installed from CRAN. `learnr` is required to 
build the shiny app, whilst `reticulate` is required for running embedded python 
sessions.

``` r
install.packages("learnr")
install.packages("reticulate")
```

- `gradethis` can be installed from GitHub. It is required for specific code 
checking and feedback. 

``` r
remotes::install_github("rstudio/gradethis")
```
