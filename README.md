# Sales Predictions
  
## Project Overview: 
Analyzing how properties of products and outlets can play crucial roles in predicting sales 

**Nokuthula Mchunu**: 

### Businesses are sitting with problem of trying to find ways of increasing their annual sales.This analyses outlines in detail what features they should focus on in relation to increase the Sales .


### Data Source: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii
For this dataset there are 8523 records, 12 columns.
 
Below is the Data Dictionary for this dataset:


![image](https://github.com/Noks06/Prediction-of-Product-Sales/assets/47742188/ba6b383c-88c9-4eee-bb16-aef9662e4c49)

## To Prepare this data set , Data was cleansed and following processes were followed.
	1. Checked and correct the inconsistancies in the dataset
	2. Checked the duplicated if found then droped 
	3. Checkedd the null values and impute them with mean value

## Results

#### Item_Outlet_Sales vs Outlet_Type
![image](https://github.com/Noks06/Prediction-of-Product-Sales/blob/main/barplot.png)

> The image shows that Supermarket Type 3 has the highest sales of more that $3500.

#### Correllation of numeric features against Item_Outlet_Sales
![image](https://github.com/Noks06/Prediction-of-Product-Sales/blob/main/Correllation.png)
>The image shows that Item_MRP has a positive correlated to Item_Outlet_Sales than other numeric featurs which have negetive correaltion 	   

## Machine learning using folowing Model:
	1. Linear Regression Model
	2. Bagging Tree Model
	3. Random Forest Model 
	4. Fine-Tuned Random Forest Model

##Models Evaluated Results:

### Linear Regression Model
------------------------------------------------------------
Regression Metrics: Training Data
------------------------------------------------------------
- MAE = 848.087
- MSE = 1,299,826.729
- RMSE = 1,140.099
- R^2 = 0.561

------------------------------------------------------------
Regression Metrics: Test Data
------------------------------------------------------------
- MAE = 802.472
- MSE = 1,187,071.833
- RMSE = 1,089.528
- R^2 = 0.570

With Linear Regression Model, the model perfom well on both set with testing set performing well showing the R^2 score 57 percent predictions
 


### Bagging Tree Model
------------------------------------------------------------
Regression Metrics: Training Data
------------------------------------------------------------
- MAE = 323.385
- MSE = 242,809.072
- RMSE = 492.757
- R^2 = 0.918

------------------------------------------------------------
Regression Metrics: Test Data
------------------------------------------------------------
- MAE = 795.922
- MSE = 1,306,988.788
- RMSE = 1,143.236
- R^2 = 0.526 
With Bagging Tree Model , the model is overfitting, it has perfom well on the training set but worse on the testing set showing the R^2 score of 
0.53 and train set R^2 Score of 0.918


### Random Forest Model
------------------------------------------------------------
Regression Metrics: Training Data
------------------------------------------------------------
- MAE = 297.494
- MSE = 183,709.103
- RMSE = 428.613
- R^2 = 0.938

------------------------------------------------------------
Regression Metrics: Test Data
------------------------------------------------------------
- MAE = 768.494
- MSE = 1,218,704.899
- RMSE = 1,103.950
- R^2 = 0.558
Default Random Forest shows again model being overfitting with result showing 0.94 on train set and 0.56 on test set


### Fine-Tuned Random Forest Model, its evaluated results:
	------------------------------------------------------------
Regression Metrics: Training Data
------------------------------------------------------------
- MAE = 756.427
- MSE = 1,157,408.215
- RMSE = 1,075.829
- R^2 = 0.609

------------------------------------------------------------
Regression Metrics: Test Data
------------------------------------------------------------
- MAE = 728.144
- MSE = 1,091,982.756
- RMSE = 1,044.980
- R^2 = 0.604

On a train and test set, both R^2 score are showing result of above 60 percent, both sets have almost same predictions
although test set predictions are below by 0.5 percent which is a small percentage.If these results are not satisfactory, more 
parameter can be added but there is not much of a change that can be seen.       

The model that can perform the prediction better is the Random Forest Model, the little bit of improvement on parameter , it can give us better results 
it has shown with the above 60 % on perfomance on both train and test set which is the better score compare to other models that were trained.  

Looking at testing set of Fine Tuned Random Forest Model:
	1. Mean Absolute Error (MAE), the model was below on its predictions by $728.14
	2. Mean Absolute Squre Error (MSE) was off by $1,091,982.756
	3. Root Mean Absolute Error (RMSE) was off by $1,044.980


## Recommendations:

For the improvement of Sales the focus should be on outlet-type as well as where the oulet is located. Supermarkets are mostly have high Sales than grocery stores   
and the reason is that mostly supermaket are located where most people are. Townships and rural areas are where most people ar located so building supermakets in those areas
can improve annual sales by far magin. 


## Limitations & Next Steps

The limitations could be crime in the populated areas. Crime involve theft, killings, robbery to mention the few. High security will be needed to combat crime.


### For further information


For any additional questions, please contact Nokuthula Mchunu the email is: **nokuthula.mchunu@momentum.co.za**
# Sales-Predictions-
