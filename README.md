# python-training
This is an interactive, online introduction to python training for employees 
in Public Health Scotland.

## Running in Posit Workbench

This project has a renv (R environment) and you can recreate the needed packages following these steps:
1. Install renv in your current R session:
``` r
install.packages("renv")
```
2. Restart your R session
3. Run this command in R console:
``` r
renv::restore()
```
4. All the required packages will be installed.
5. If the restore process fails you can install required R packages running these lines of code in your R console:
``` r
install.packages("learnr")
install.packages("reticulate")
```

### R required packages


| Package | Description |
|---------|---------|
| learnr | It is required to build the shiny app |
| reticulate | It is required for running embedded python sessions |

### Python required packages

The required Python are available in requirements.txt file. No need to install since reticulate R package manages the required virtual environment installation.

| Package | Description |
|---------|---------|
| pandas | It is required to read files (e.g. CSV) and wrangle its content |


### Troubleshooting

- If PWB has been updated it means there are new Python versions. So you have to 
check if your previously created pyenv is still there. Run this command in the 
terminal tab: `ls -l ~/.virtualenvs`
- If you see pyenv folder, you have to delete it using this command: 
`rm -rf ~/.virtualenvs/pyenv`
- The previous pyenv gets obsolete because of a PWB update with new Python 
versions.
- We will be able to run this project because it will create a new pyenv 
(with the new Python version).

## Deployment

This project can be deployed in Posit connect. You will need an API token and the URL if it has already been installed.
