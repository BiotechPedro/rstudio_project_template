This is the basic structure I plan to follow for all my projects starting later than 2022-10-20. It relies on `cookiecutter` and the structure is the following.

### Project organization
-----------

    ├── analysis                           <- qmd files containing the code for the analyses. Naming convention is a number (for ordering) with a short (`-` delimited) description, e.g. `01-Exploratory-Analysis.qmd`. 
    │   └── index.qmd
    ├── code                               <- Non-R scripts that will be used in this project
    ├── {{ cookiecutter.repo_name }}.Rproj <- Create Rstudio project
    ├── data                               <- Any kind of data (raw, processed, output from pipelines, etc) that will be used for the project
    ├── docs                               <- Rendered html reports of qmd files
    ├── misc                               <- Other files
    ├── output                             <- Output plots and files from qmd files
    ├── _quarto.yml                        <- Configuration of Quarto settings, html display, webpage, etc.
    ├── README.md                          <- The top-level README for developers using this project.
    ├── src                                <- Source code for use in this project (R)
    ├── styles.css                         <- CSS file to style the webpage
    └── theme.scss                         <- SCSS file to style the webpage


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5+
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
--------------------------------

    cookiecutter https://github.com/BiotechPedro/rstudio_project_template
