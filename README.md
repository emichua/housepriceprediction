## Ames Housing Data

We are a group of home improvement consultants that provide suggestions on how to refurbish the houses in selected neighborhoods in Ames, Iowa, including selecting the best features for homeowners to renovate, in order to improve the value of their homes in a cost-effective way.

To help predict which feature to improve in order to increase housing price, I will create a linear regression model based on the Ames Housing Dataset. 

The problem statement is -

**In order to let seller sell their property for higher price in the future, which housing features to improve?**

Besides, I also will find out which model can give the most accurate predictions of sales price with the selected features.

### Datasets:
The Ames Housing dataset contains 2000 entries of properties with 80 over descrete, nominal & ordinal features in Ames, Iowa. The properties were sold between 2006-2010.
The detailed description is shown in this link below:
http://jse.amstat.org/v19n3/decock/DataDocumentation.txt

### Tables of content:
1. Abstract
2. Import and loading data
3. Exploratory data analysis
4. Data cleaning
5. Feature Engineering
6. Data Visualization
7. Data Modelling
8. Model fitting & Evaluation
9. LINE Assumptions
10. Conclusions & Recommendations

### 1. Abstract
Overview:

1) Exploratory Data Analysis:
Numerical features - a heatmap and correlation coefficients are used to show the linear relationship.
Categorical features - box plots are used to the relationship between Sale Price and categories.

2) Feature Engineering: 
Amplify signal of categorical data for better accuracy when fit in model.

3) Data Modelling: 
Linear Regression, LASSO and Ridge models are used for comparison. 
Lasso was used to select and narrow down features 
Models were evaluated and selected based on RMSE score. 
Ridge model is chosen as final model.

My model is able to predict housing prices with an error of $23,910.

The top 5 features for sellers to achieve the highest selling price -

- Overall quality and living area 

- Basement square feet

- Lot size 

- Excellent exterior quality

- Excellent kitchen quality            

However, not all the features listed above are able to be changed, eg: basement square feet. We can only pick those features which are improvable like exterior quality and kitchen quality. Since 3 out of 5 features are not changeable, I have extended the list to show features which have $600 coefficient and above to maximise the ROI.

For 2-8, please refer my notebook `project_2 Ames housing predictive modelling`

### LINE Assumption:
Linearity - passed
Independence - passed
Normal distribution - passed
Equal variance of residuals - failed

### Conclusions & Recommendations
#### In conclusion, in order to sell at higher price for home improvement, we have to choose the features where we can change which are the categorical features as we can't increase the lot area and change the built year. 

These are the features* to look into when it comes to home improvement:

1. Excellent exterior quality $6608 increase in sale price

2. Excellent kitchen quality results in $5740 increase in sale price

3. Excellent basement quality results in $4441 increase in sale price

4. Good basement exposure results in $3995 increase in sale price

5. Good quality of materials used on exterior results in $2878 increase in sale price

6. Having a fireplace results in $2427 increase in sale price

7. Excellent heating quality & condition results in $2271 increase in sale price

8. Having a central air results in $1432 increase in sale price

9. Having good quality of fireplace results in $1428 increase in sale price

10. Having Good living quarters for basement finished area results in $965 increase in sale price

11. Newly renovated properties results in $885 increase in sale price

*Assume that other features are constant

Besides, the neighbourhood which can be considered to buy is Northridge Heights as it can result in $2036 increase in sale price.