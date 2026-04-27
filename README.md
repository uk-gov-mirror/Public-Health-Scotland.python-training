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

# Running in Posit Workbench
- If PWB has been updated it means there are new Python versions. So you have to 
check if your previously created pyenv is still there. Run this command in the 
terminal tab: `ls -l ~/.virtualenvs`
- If you see pyenv folder, you have to delete it using this command: 
`rm -rf ~/.virtualenvs/pyenv`
- The previous pyenv gets obsolete because of a PWB update with new Python 
versions.
- We will be able to run this project because it will create a new pyenv 
(with the new Python version).
