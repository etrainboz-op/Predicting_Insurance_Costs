# Predicting Healthcare Insurance Charges: A Comparative Analysis of Regression and Machine Learning Models

This project investigates how well individual healthcare expenses can be predicted using demographic and lifestyle variables. The analysis is based on a publicly available data set that can be found on *Kaggle* through a link contained in the "References" section in the project report. Common machine learning models like simple and multiple linear regression, as well as decision trees and random forests were performed. A logarithmic transformation of the response variable was used to address skewness and improve model performance. Model evaluation was conducted using training and test data, with metrics such as RMSE and R-squared used to compare predictive accuracy. Results indicate that smoking status, age, and BMI are the most influential predictors of insurance charges, with smoking having the strongest effect. Overall, this analysis highlights the effectiveness of combining statistical and machine learning techniques to model healthcare costs and provides insight into the key factors that influence insurance pricing.

## Files

This project was accomplished through R Studio where each contributing file has an R markdown extension along with a pdf copy. 

### Data Set

File: `insurance.csv`

The data set for this project contained seven variables of 1,338 observations. These variables include age, sex, BMI, geographical region, smoking status, number of children, and the response variable charges.

| **Variable** | **Type** | **Description** |
|--------------|----------|-----------------|
| **Age** | Explanatory | Quantitative variable being the age of someone in integer years |
| **Sex** | Explanatory | Qualitative variable of an individual either being male or female |
| **BMI** | Explanatory | Quantitative variable being the measure of a persons body fat based on height and weight |
| **Children** | Explanatory | Qualitative variable of the number of children that an individual has |
| **Smoker** | Explanatory | Qualitative variable if someone is a smoker or not |
| **Region** | Explanatory | Qualitative variable of the region an individual resides in the United States |
| **Charges** | Response | Quantitative variable being how much a person is charged in medical insurance |

### EDA

Files: `EDA.Rmd` `EDA.pdf`

Contains work for exploratory data analysis before any model was created. This includes data preperation, cleaning, variable transformations, and nummerical/visual summaries.

### Simple Linear Regression

Files: `SimpLinModels.Rmd` `SimpLinModels.pdf`

Used simple linear regression of each variable against charges for baseline results and simple interpretation. 

### Multiple Linear Regression

Files: `MultLinModels.Rmd` `MultLinModels.pdf`

These files contain the multiple linear regression models that aimed to decrease model error using combinations of variables and interaction terms.

### Decision Trees and Random Forests

Files: `TreeModels.Rmd` `TreeModels.pdf`

With the presence of many qualitative variables, decision trees were modeled to create very interpretable results while still preserving minimal error. These algorithms were especially helpful for dealing with variables where linearity could not be assumed. Likewise, random forests were used to find even lower RMSE values but with a tradeoff in interpretation. 

### Report

Files: `Project.Rmd` `Project.pdf`

Shows the final written report in raw markdown, or in the exported pdf format.
