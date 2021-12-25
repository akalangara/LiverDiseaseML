# Project Description

Infection by a viral agent, can result in inflammation of the liver, broadly called Hepatitis. This can progress further to fibrosis, the scarring of liver tissue; and further still to cirrhosis, late stage scarring that impairs liver function. It is important to monitor liver disease progress and the gold standard for liver fibrosis evaluation is liver biopsy; though this is an invasive procedure. In contrast, blood work is minimally invasive, conducted routinely, and specific liver function blood panels have been developed to help with assessing liver function. This report aims to develop a multinomial logistic regression model that utilizes blood lab results, as well as patient characteristics like age and biological sex, to accurately classify the progression of liver disease.

## Generate Report Using Renv
<details>
  <summary>Instructions</summary>
  
  ### Necessary Programs
  For this analysis it is necessary to have R and the libcairo2-dev package installed on Ubuntu.
  You can use the following code to install the libcairo2-dev package.
  ```bash
  sudo apt-get update -y
  sudo apt-get install -y libcairo2-dev
  ```

  ### Restore Package Environment
  Prior to executing the analysis, navigate to the `LiverDiseaseML` directory and start an R session
  ```bash
  R
  ```
  In the R session, run the following to restore the package environment
  ```R
  renv::restore()
  ```
  There may be a lot of output. Please note any errors or warnings of uninstalled packages that come up.
  Quit the R session once this step is completed.
  ```R
  q()
  ```
  ### Execute Analysis
  To execute the analysis, from the `LiverDiseaseML` directory, run the following
  ``` bash
  Rscript -e "rmarkdown::render('FinalProject.Rmd', output_file = 'Output/MLReport.pdf', quiet = TRUE)"
  ```
  This will create in the `LiverDiseaseML/Output` directory, a file called `MLReport.pdf` which contains a report of the findings.
  Please note that any errors about convergence can be ignored.
</details>

