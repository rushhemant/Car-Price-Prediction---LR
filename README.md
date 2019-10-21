# Car-Price-Prediction---LR
Determine - 
Which variables are significant in predicting the price of a car
How well those variables describe the price of a car

**Read Data**	
* Import important libraries	
* Read application data file into dataframe	
* Shape of car_data dataframe	
* Quick review of car_data dataframe	
	
**Data Cleaning**	
* Analyze columns for missing values in car_data	
* Split CarName into Name and Model	
* Check data for any discrepancy	
* Correct car company name	
	
**Univariate Analysis**	
* Analyze outliers from quantitative variables	
* Remove outliers from car_data	
* Bar plots of quantitative variables vs price	
	
**Segmented Univariate Analysis**	
* Analyze impact of categorical values on price of car	
	
**Bivariate Analysis**	
* Checking correlation of quantitative variables in car_data	
	
**Feature Engineering**	
* Create new variable lbh = length * width * height	
* Create new variable hplevel (horsepower level)	
* Create new variable citympg (citympg level)	
* Create new variable powtoweight = horsepower/weight	
* Create new variable lwratio = carlength/carwidth	
* Create new variable lhratio = carheight/carlength	
	
**Data Preparation for Modeling**	
* Drop car_id and CarName	
* Label encoding for doornumber and cylindernumber	
* Dummy variable encoding (one-hot) for other categorical variables	
* Splitting the Data into Training and Testing Sets	
* Scaling the variables using MinMaxScaler (Normalizing)	
	
**Model Building**	
* Create X and y sets	
* Using RFE for feature selection	
* Build model1 thru model7	
* Residual Analysis - Distribution of error terms	
	
**Evaluation of Model**	
* Transform/scale test dataframe	
* Prediction on test set	
* Calculate r2 for test set	
	
**Conclusion**	
