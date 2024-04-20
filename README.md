# Rape-Reported in India Repository

## About:
This is a mini project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses the prediction of number of rape reported all 35 states of India from 2001-2010 using a trifactor approach: Police Complaints, Police Corruption, and Police Strength. 

The mini project implements the data pipeline (except Ethical Consideration): Sample Collection, Data Preparation, Exploratory Analysis, Analytic Visualisation, Algorithmic Optimisation, Information Presentation, and Ethical Consideration.

For a detailed walkthrough, please view the source code in order from:
1. [ReadMe File](https://github.com/ZaydShabazAli/SC1015MiniProject/blob/main/README.md)
2. [Analysis of Factor 1](https://github.com/ZaydShabazAli/SC1015MiniProject/blob/main/Police_Complaints_Barnabas.ipynb) (Police Complaints)
3. [Analysis of Factor 2](https://github.com/ZaydShabazAli/SC1015MiniProject/blob/main/Police_Corruption_Zayd.ipynb) (Police Corruption)
4. [Analysis of Factor 3](https://github.com/ZaydShabazAli/SC1015MiniProject/blob/main/Police_Strength_KeJun.ipynb) (Police Strength)


## Contributors:
@ClassicalAI - Police Complaints

@ZaydShabazAli -  Police Corruption

@yeokjunn - Police Strength

## Problem Definition
How and what can we use to predict the number of rape cases reported in India by state from 2001-2010, based on various factors (Police Complaints, Police Corruption, and Police Corruption)?
Which machine learning model is the best to predict it?

## Machine Learning Models Used
Police Complaints:
K-Nearest Neighbours
Ridge Regression
Support Vector Machines

Police Corruption:
Linear Regression
K-Nearest Neighbours
Neural Networks

Police Strength:
Linear Regression
Polynomial Regression
K-Nearest Neighbours

## Police Complaints Conclusion
As Rape Reported & Complaints_Received/Alleged has a strong correlation of 0.71, indicating a strong linear relationship, Complaints_Received/Alleged is an important predictor of Rape Reported.
Out of the three machine learning models implemented (KNN: Mean Squared Error - 392774666.08746356; Ridge Regression - Mean Squared Error: 125688531.65739381; SVM: Mean Squared Error - 36334198.68137042), SVM has the smallest Mean Squared Error, and is thus the best machine learning model in terms of predicting Rape Reported using Complaints_Received/Alleged.

## Police Corruption Conclusion

## Police Strength Conclusion
Police Strength per state and Rape Cases reported has a rather weak correlation of -0.16, which indicates that as Police Strength per state increases, rape cases reported decreases.

After using 3 different machine learning methods, I have found that the polynomial regression method (8th degree) is the best predictor of our response variable, with an explained variance of 0.49, compared to other methods such as linear regression (explained variance of 0.06) and K-Nearest Neighbours (explained variance of 0.38). Values of explained variance are calculated after removal of outliers from the dataset, for all 3 machine learning methods.

## Conclusion
Out of the three predictors (Police Complaints, Police Corruption, Police Strength), the strongest predictor for Rape Reported is Police Complaints, which has the highest absolution correlation value of 0.71 as compared to Police Corruption: 0.16, and Police Strength: 0.42. Police Corruption is the weakest predictor for Rape Reported.

For the strongest predictor, Police Complaints, the best (most accurate) machine learning model is Support Vector Machines (see Police Complaints Conclusion). 

To best predict the number of rape cases reported in India by state from 2001-2010, Support Vector Machines model with the predictor variable: Police Complaints can be used. As a second best alternative, the Linear Regression model with the predictor variable: Police Corruption (see Police Corruption Conclusion) can be used. 

## What did we learn from this project?
1)Using multiple datasets, extracting variables with different indexes, and merging them properly for accurate analysis

2)Applying data cleaning for large datasets with > 1700 rows for some datasets

3)Removal of outliers from the dataframe using methods such as Z-Score, and Inter-Quartile Range (IQR)

4)New Machine Learning Methods:
Neural Networks, K-Nearest Neighbors, Polynomial Regression, Ridge Regression, Support Vector Machines

5)Collaborating with GitHub Repositories

## References
