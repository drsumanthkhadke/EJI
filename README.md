Environmental Justice and Respiratory Health Analysis
Overview
This R code analyzes the relationship between environmental justice indicators (EJI) and respiratory health outcomes (asthma and COPD) across different geographic regions. The analysis incorporates demographic data, environmental burden metrics (EBM), and social vulnerability metrics (SVM).

Dependencies
The code requires the following R packages:

tidyverse
DescTools
readxl
Data Sources
The analysis uses several data files:

PLACES.csv - Contains health outcome data
EJI.csv - Environmental Justice Index data
Age_US.xlsx - Age demographics
RaceUS.xlsx - Race demographics
hispanicUS.xlsx - Hispanic population data
nonhispanicUS.xlsx - Non-Hispanic population data
ruralurbancodes2013.xls - Rural-Urban classification codes
Key Features
Data preprocessing and merging of multiple demographic datasets
Creation of categorical variables for EJI, EBM, and SVM levels
Population-adjusted analysis using offset terms
Stratified analysis by rural/urban status
Multiple regression models examining:
Unadjusted associations
Age-adjusted associations
Fully adjusted models including smoking, healthcare access, and demographic factors
Analysis Components
Descriptive statistics for population characteristics
Poisson regression models for disease prevalence
Interaction analyses between environmental and social vulnerability metrics
Stratified analyses by environmental burden levels
Output
The code generates:

Risk ratios with confidence intervals
Stratified prevalence estimates
Adjusted association measures between environmental justice indicators and respiratory outcomes
Usage
Ensure all required data files are in the working directory
Install required R packages
Run the code sequentially to reproduce the analysis
Notes
Missing data is handled using complete case analysis
Population counts are used as offset terms in regression models
Geographic identifiers are standardized using leading zeros for proper merging
Contact
For questions about the code or analysis, please open an issue in the repository.

C
