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
* Features that drive the car price
* aspiration - turbo car costlier than standard car (aspiration_turbo)
* drivewheel - rear wheel drive costlier than otherr categories (drivewheel_rwd)
* enginelocation - rear engine location is thrice as costlier as front (enginelocation_rear)
* enginetype - dohcv are significant costlier (enginetype_dohcv)
* fuel system - mpfi are coslier car (fuelsystem_mpfi)
* bmw, mercury, porsche, buick and jaguar are costlier car ('carcompany_bmw','carcompany_buick','carcompany_jaguar').

* Equation for car price based on best fit line is 
𝑝𝑟𝑖𝑐𝑒=4307.98+2118.5934×𝑑𝑟𝑖𝑣𝑒𝑤ℎ𝑒𝑒𝑙(𝑟𝑤𝑑)+20500×𝑒𝑛𝑔𝑖𝑛𝑒𝑙𝑜𝑐𝑎𝑡𝑖𝑜𝑛(𝑟𝑒𝑎𝑟)+17160×𝑐𝑎𝑟𝑤𝑖𝑑𝑡ℎ+1972.3109×𝑓𝑢𝑒𝑙𝑠𝑦𝑠𝑡𝑒𝑚(𝑚𝑝𝑓𝑖)+11150×𝑐𝑎𝑟𝑐𝑜𝑚𝑝𝑎𝑛𝑦(𝑏𝑚𝑤)+12070×𝑐𝑎𝑟𝑐𝑜𝑚𝑝𝑎𝑛𝑦(𝑏𝑢𝑖𝑐𝑘)+12420×𝑐𝑎𝑟𝑐𝑜𝑚𝑝𝑎𝑛𝑦(𝑗𝑎𝑔𝑢𝑎𝑟)
