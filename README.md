# Prediction of immigrants in Spain using machine learning to forecast international migration flows.
*Note: Each step was developed separately in a jupyter notebook, which are available in the “Notebooks” folder associated with this project.*
## Specific Objectives
- List the most relevant countries in terms of foreign immigration to Spain.
- Obtain a predictive model with a coefficient of determination close to or higher than 0.80 (functional). 
- To discuss the importance of variables.
## Data Sources
For the predictive model, we took a "macro" approach to the migrant flow phenomenon. This means that we focused on including data from macroeconomic, social, political, freedom/rights, security, and other factors to model the different inherent conditions in each country that impact the decision to emigrate to Spain.
- Spanish National Institute of Statistics.
- International Organization for Migration.
- CLIMB Database.
- International Organization for Standardization (ISO).
- World Bank Group. GDP - Inflation - Country Risk.
- International Monetary Fund.
- Our World in Data.
- International Institute for Democracy and Electoral Assistance.
- United Nations Office on Drugs and Crime.
- Intentional Homicides database.
  
## Procedure
Taking into account the variety of datasets in our study and the particular need for cleaning/preprocessing of each one, it was decided to divide the project into 4 phases (see image below) that would provide an orderly sequence of cleaning, analysis, and testing of machine learning algorithms:
- Stage 1: Focused on working with Spanish immigration data segregated by demographic variables.
- Stage 2: Focused on predictor variables.
- Stage 3: Union of all data sets for variable selection analysis.
- Stage 4: Machine learning.

![image](https://github.com/user-attachments/assets/fba99f64-2be4-4830-86f7-febf8d27cff2)

In Stage 1 (E1), the initial cleaning, preprocessing, and exploration of the immigration data sets was carried out, obtaining the first insights and the top countries in number of immigrants to be included in the model. Then, based on the observations and top countries obtained in Stage 1, the cleaning, preprocessing, and analysis of the different data sets of the predictor variables began (Stage 2 - E2), exporting the preprocessed data sets from both stages.

Subsequently, we proceeded with the union of all predictor variables to the central dataset of immigration data (Stage 3 - E3), the inclusion of three additional categorical variables related to identifying Spanish-speaking countries and the pandemic/post-pandemic period (2020-2021 and 2022, respectively), and feature selection through the study of correlations and hypothesis testing.

Finally, with the data exported in Stage 3, algorithms based on linear, tree, and neural network models of one or two layers were tested (Stage 4 - E4), comparing different metrics to observe the performance of the models, identify the best ones, make the necessary parameter adjustments and distribution transformation (to normal) to reduce the error until the one with the best possible performance was obtained. Then, it was exported with the other applicable files (scaling and/or transformation) to make predictions, including the estimation of a 90% confidence interval.
