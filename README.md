# Spatial-Inequality-Air-Conditioning-
The following repository contains the code and analysis for the research paper titled: The Price of Cool: Using Hedonic Modelling to Assess Spatial Inequalities of Air Conditioning in Madrid. The data for the study is not openly available and is provided by idealista as part of a PhD collaboration, thus one year of data that has been publically publised by idealista can be replaced with our data if you would like to replicate the analysis (Madrid_Sale (2).csv)


## Notebook 1:
Data Preparation
The following notebook prepares and cleans the housing listings data provided privately by idealista for the analysis of spatial inequalities of air conditioning. Key steps in this notebook include data cleaning, and the spatial join with neighbourhood level census variables to create the dataframe for the hedonic analysis in notebook 3.

## Notebook 2:
Data Preparation for Hedonic Regression Modelling
The following analysis includes an examination of multi-colinearity between the variables for the study, which is an important step in the preparation of data for linear hedonic modelling. Multicollinearity can make it difficult to interpret regression coefficients, as it causes large standard errors, which can result in insignificant predictors even when they are important.
It doesn't affect the predictive power of the model but complicates understanding the relationship between predictors and the response variable. Multicollinearity occurs when two or more predictor variables in a regression model are highly correlated, which can make it difficult to determine the individual contribution of each predictor to the dependent variable.

We also transform variables so the scale of variables doesn't impact the coefficients.

## Notebook 3:
Fit Hedonic Regression Models
This notebook fits the hedonic house price regression models and calculates the model statistics. Six models are fitted which incrementally add different types of predictor variables and interaction effects. Finally, the point data is joined to administrative polygons and exported to fit the final multi level models in R.
