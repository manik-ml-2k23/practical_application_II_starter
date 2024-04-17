# papp2

## Background:
what drives a price of a Car?
The goal of this project is to explore used vehicles dataset from Kaggle and understand what factors make a car more or less expensive.  


## Solution submission:
Papp_II.ipynb - Contains the solution sumbission

## Data Exploration:

### Data Info:
Provided vehicles.csv data has 426880 and total of 18 columns.

### Missing Data:
As first step the data was analyzed for missing values and nans. Missing data are summarized below.

id                   0
region               0
price                0
year              1205
manufacturer     17646
model             5277
condition       174104
cylinders       177678
fuel              3013
odometer          4400
title_status      8242
transmission      2556
VIN             161042
drive           130567
size            306361
type             92858
paint_color     130203
state                0



## Data cleaning:

- 'VIN', 'region', 'state' columns were dropped as they are not related to feature of a car 
- NANs were dropped after first evaluating the model by keeping all the data as prediction indicated by RMSE and R-Squared were poor
- The cleaned data was then left with 34868 entries. While this is significant drop from the original dataset, this still seems sufficient representation of data

## Data Visualization:

#### Box plot of vehicles by manufacturer reviweing one categorical vs conitnuous variable of price
- We can see traditional luxury cars have high price from manufactures of Ferrari, Porsche, Aston-Martin
- Electric vehicles by Tesla are priced higher over most gas based vehicles
- Majority of the vehicles are under 20K


![alt text](images/boxplot.png)


## Analysis and Modeling

- Exploratory Data Analysis (EDA): Analyzed the dataset to understand data distributions, correlations, and relationships between features.
- Data Preprocessing: Handled missing values and outliers
- Machine Learning Models: Linear regression and Lasso regression for predicting vehicle prices using cross validation
- Model Evaluation: Evaluated model performance using RMSE and R-squared

## Dependencies

The analysis and modeling require following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn


## Next Steps:
As per CRISP-DM, the next step would be to deploy the recomendation provided and monitor and fine tune as necessary and use as feedback for future modeling.