# Predicting the outcome of a PCR test for COVID-19 using a routine blood exam: A replication

#### -- Project Status: Completed

## Project Objective

The purpose of this project is to replicate the Random Forest, Decision Tree and Logistic Regression classifiers of the following study [1].

### Methods used

- Machine Learning
- Multiple Imputations using Chained Equations
- Data Visualization

### Technologies

- R
- Python
- pandas, scikit-learn, numpy, jupyter, rpy2, matplotlib, seaborn, mice

## Setup Instructions

- Use .yml file to create environment (this installs all required packages including rpy2)
- How to setup rpy2 to work with R
  - R has to be installed on the computer and setup properly in the system variables (user variables should suffice)
  - additionally, the 3 following variables should be set up as user variables
    - R_HOME is set to the path of the R installation, e.g., 'C:\Program Files\R\R-{version-number}'
    - R_LIBS_USER set to the library path where R installs some (or all) of the packages, e.g., 'C:\Users\\{username}\Documents\R\win-library\\{version-number}'
    - R_USER set to the path of the rpy2 installation, e.g., 'C:\Users\\{username}\anaconda3\envs\\{env-name}\Lib\site-packages\rpy2'
  - now the mice package can be installed in R using, e.g., the R console
  - the package should now be useable
  - sometimes ryp2 and R are not able to find all libPaths (directories where R packages are installed), this can be added as shown in the first code cell of the ba_code.ipynb notebook

## Repository structure

```
|-- ba
    |-- .gitignore
    |-- README.md
    |-- ba.yml
    |-- blood-exams
    |   |-- covid_study.xlsx
    |   |-- covid_study_v2.xlsx
    |-- notebooks
        |-- ba_code.ipynb (contains the code used to clean the data, train, evaluate and validate the models)
        |-- eda_blood_italy.ipynb (examines the data set in an exploratory fashion)
        |-- result_viz.ipynb (code to generate summaries and plots used during evaluation and validation)
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

## References

[1] Brinati, D., Campagner, A., Ferrari, D., Locatelli, M., Banfi, G., & Cabitza, F. (2020). Detection of COVID-19 Infection from Routine Blood Exams with Machine Learning: A Feasibility Study. Journal of Medical Systems, 44(8). [doi:10.1007/s10916-020-01597-4](https://doi.org/10.1007/s10916-020-01597-4)
