# Code for Bachelor's thesis

## Contents
1. [How to install the environment](#How-to-install-the-conda-environment)
2. [Repository structure](#Repository-structure)

-------

### How to install the conda environment
- Use .yml file to create environment (this installs all required packages including rpy2)
- How to setup rpy2 to work with R
    - R has to be installed on the computer and setup properly in the system variables (user variables should suffice)
    - additionally, the 3 following variables should be set up as user variables
        - R_HOME is set to the path of the R installation, e.g., 'C:\Program Files\R\R-{version-number}'
        - R_LIBS_USER set to the library path where R installs some (or all) of the packages, e.g., 'C:\Users\\{username}\Documents\R\win-library\\{version-number}'
        - R_USER set to the path of the rpy2 installation, e.g., 'C:\Users\\{username}\anaconda3\envs\\{env-name}\Lib\site-packages\rpy2'
    - now the mice package can be installed in R using, e.g., the R console
    - now should be able to use package

### Repository structure
```
|-- ba
    |-- .gitignore
    |-- README.md
    |-- ba.yml
    |-- blood-exams
    |   |-- covid_study.xlsx
    |   |-- covid_study_v2.xlsx
    |-- notebooks
        |-- ba_code.ipynb
        |-- eda_blood_italy.ipynb
        |-- result_viz.ipynb
        |-- figures
        |   |-- density_no_split.jpg
        |   |-- density_plots.jpg
        |   |-- dt.png
        |   |-- dt_importance.png
        |   |-- imputed.png
        |   |-- imputed_only.png
        |   |-- lr_exp.png
        |   |-- lr_importance.png
        |   |-- lr_importance_abs.png
        |   |-- prc.png
        |   |-- rf_importance.png
        |   |-- roc.png
        |-- imputed_sets
        |   |-- imputed0.csv
        |   |-- imputed1.csv
        |   |-- imputed10.csv
        |   |-- imputed11.csv
        |   |-- imputed12.csv
        |   |-- imputed13.csv
        |   |-- imputed14.csv
        |   |-- imputed15.csv
        |   |-- imputed16.csv
        |   |-- imputed17.csv
        |   |-- imputed18.csv
        |   |-- imputed19.csv
        |   |-- imputed2.csv
        |   |-- imputed20.csv
        |   |-- imputed21.csv
        |   |-- imputed22.csv
        |   |-- imputed23.csv
        |   |-- imputed24.csv
        |   |-- imputed3.csv
        |   |-- imputed4.csv
        |   |-- imputed5.csv
        |   |-- imputed6.csv
        |   |-- imputed7.csv
        |   |-- imputed8.csv
        |   |-- imputed9.csv
        |-- metrics
            |-- eval_storage.csv
            |-- eval_storage.tex
            |-- imputed.csv
            |-- imputed.tex
            |-- lr.txt
            |-- masked_imputed.tex
            |-- rf.txt
            |-- u_imputed.tex
            |-- val_storage.csv
            |-- val_storage.tex
```