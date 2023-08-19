# Prediction-of-Product-Sales
- Author: Deshan Pillay
### Business problem:
- Predict the sales for food items which are sold at various stores.
- To help the retailer understand the properties of products and outlets that play crucial roles in increasing sales.
### Data:
- Source: The business provided a CSV file containing the below information:
 1   Item Weight                
 2   Item Fat Content          
 3   Item Visibility           
 4   Item Type               
 5   Item MRP                   
 6   Outlet Identifier          
 7   Outlet Establishment Year   
 8   Outlet Size                 
 9   Outlet Location Type       
 10  Outlet Type                
 11  Item Outlet Sale

## Methods
* Load,inspect and clean the data
   - Import required numpy and pandas libaries
   - Check how many rows and columns
   - Verify the datatypes
   - Check for duplicates
   - Identify missing values and address by using a place holder
   - Find and fix inconsistent categories of data
   - Obtain statistics for numerical columns
     
* Exploratory Data Analysis
   - Use the below statistical analyses to help understand the data
   - Histograms to view the distribution of numerical features
   - Boxplots to view statitical summaries of numerical features
   - Countplots to view the frequency of each class of categorial features
   - Heatmap to view the correlation between features.

* Explanatory Data Analysis
  - Item Outlet sales was used as the target
  - Use univariate visualization to show the distribution of values/categories
  - Use multivariate visualization plotting each feature vs the target
 

## Results

![Total Sales for Outlets](https://github.com/Desh86/Prediction-of-Product-Sales/assets/138576166/7a661635-d45e-4654-a536-91c37faf7aec)

This visual indicates the number of outlets and the total sales each one makes, the higher the sales the fewer the outlets.

![image](https://github.com/Desh86/Prediction-of-Product-Sales/assets/138576166/d2fea62b-b9ed-48f0-b9f1-da97e83bbf12)

This visual indicates number of sales by the tyoe of Outlet, Supermarket Type 1 makes the most sales.

![image](https://github.com/Desh86/Prediction-of-Product-Sales/assets/138576166/347e8fbb-9811-4064-81d4-b17a7319af64)

This is a heatmap which indicates the correlation. The closer the value to 1 the higher the correlation ( Item MRP and Item Outlet sales have a correlation)

![image](https://github.com/Desh86/Prediction-of-Product-Sales/assets/138576166/37692328-b520-4412-ab14-b60561abfb10)

This is a scatter plot which indicates the sales vs the location of the store and grouped by the outlet type. Supermarket type 3 makes the most sales in the location Tier 3

![image](https://github.com/Desh86/Prediction-of-Product-Sales/assets/138576166/a968e3a3-3192-4460-b9f5-8de6247b6122)

This is a numeric feature with a high cardinality.

![image](https://github.com/Desh86/Prediction-of-Product-Sales/assets/138576166/a7495af5-160d-43a7-accb-b5fb772a9f03)

This model shows outliers on Low Fat which will effect the target.


## Model
The Random Forest Regression Metrics was applied to the model.
  - The Random Forest model showed a higher R^2 value when using GridSearchCV to tune the hyperparameters.
  - Random Forest are reliable and effective.
  - Random Forest fit data better from the get go without the transforms.
  - You dont need to scale the data and often dont need to remove outliers.
Based on the Test data, we can determine the below:
MAE,MSE and RMSE were lower than the training data
R^2 had a higher value in the test data vs the training data.
The test data performed better than the training data.
The R-Squared results in the model indicates that 59% of the variation in the outcome is explained by the model, the remaining 41% is due to other factors or random error.


## For further information:
For any additional questions, please contact desh.pillay@gmail.com





