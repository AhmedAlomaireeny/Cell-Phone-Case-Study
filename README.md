# Cell-Phone-Case-Study
## 1.	Project description
In Digital Cell manufactures a broad line of phones for the consumer market. The chief operations officer, has asked Paul who has just been hired as a management analyst to do an assignment about the stock of the end of each month, handing the analyst a table that shown here the actual order entered for the three years with 144 phones per case.

The COO wants to know what the business will look like over the next 6 to 12 months by creating a report using regression analysis, providing a summary of the cell phone industry outlook and how does the analysis change by adding seasonality into the model.

![image](https://user-images.githubusercontent.com/124380622/216650864-8b608014-cf29-4976-900c-f16cc0c204f6.png)

## 2.The solution methodology
We approach the solution using regression analysis ( least square method ) it helps us to minimize the sum of squared errors.
   
We the received orders data by month from 2007 to 2009 to calculate forecasted demand for the next 6 to 12 months without adding seasonality into our model for the first method. 

To calculate the forecasted demand using regression analysis we need to find y-axis intercept ( a ) and the slope of the regression line ( b )
We need to use the following equations to calculate the demand at a given month :  

Equation 1 Linear regression:

![image](https://user-images.githubusercontent.com/124380622/216651636-3a55117c-8a05-4c2b-918f-f6d7967d986d.png)

where :
y = computed value of the variable to be predicted (dependent variable) 
a = y-axis intercept 
b = slope of the regression line 
x = the independent variable

To calculate a and b we need to use the following equations :
Equation 2 Slope

![image](https://user-images.githubusercontent.com/124380622/216651581-64e59092-8519-46c9-9fc5-6b0f1733f991.png)


Equation 3 y-axis intercept:

![image](https://user-images.githubusercontent.com/124380622/216651738-281d7624-23a8-494e-ba57-dbdf2a086ee3.png)

Where : Xbar and Ybar are the months mean and cases mean respectively 
We used Microsoft Excel to organize the date and to do the needed calculations and the data as follow :

![image](https://user-images.githubusercontent.com/124380622/216651814-056e580f-25d9-4397-889c-948be1872d2f.png)

![image](https://user-images.githubusercontent.com/124380622/216651853-50dc0bcf-b5a4-4367-b0a0-004d5c6164a7.png)

![image](https://user-images.githubusercontent.com/124380622/216651884-ae34775e-48f2-494a-b1dc-4fd39785d5e8.png)


From the tables above we calculated the following : 

![image](https://user-images.githubusercontent.com/124380622/216652042-6a17bbd7-874d-4879-8bc4-7283d1c8e1cf.png)
   
**We get b = 5.24839 and a = 440.849 and thus,**
**y=440.95+5.25x**

![image](https://user-images.githubusercontent.com/124380622/216652694-e2843537-b50e-44d3-9769-9df8c12c785a.png)

# Method 2
In method 2 we include seasonality, so we need to calculate the seasonal index using the avg yearly demand and the avg monthly demand using the following equations: 

**Equation 4 Avg monthly demand:
Avg monthly demand=(Total avg yearly demand)/12**

**Equation 5 Seasonal indix 
Seasonal Index=Avg yearly demand of month i/Avg monthly demand**

**Forcast=Avg monthly forcasted demand x Seasonal index** 

**Also, we need forecasted yearly demand of year 4 ( 2010 ) and we get it from table 5**

## 3.	The results and recommendations

## For Method 1 
we used least square method to find the trend line and we used the trend line to forecast the demand for the next year which is from month 37 to month 48 and we got the following results : 

![image](https://user-images.githubusercontent.com/124380622/216653652-f150280f-b436-4dd1-a774-1c3a1f14df82.png)

**We see that the from the trend line and the forecasted demand that the demand is increasing continuously over the years we recommend the Digital Cell Phone to increase there production of the cell phone and manage the inventory to meet that continuous change in demand we advise them to Lead the demand with incremental expansion to avoid stockouts**

## For method 2 
We added seasonality into our model which required to calculate the seasonal index and the yearly demand of year 2010 which we get from 

![image](https://user-images.githubusercontent.com/124380622/216653808-34d9ee27-f382-4c2f-a91f-98fe3c13498c.png)

**We see that December has the highest seasonal index and the highest forecasted demand with around 9.553% demand more than the avg we conclude that we get the highest demand in the year around December ( also we get high demand in January and November ) so we advise Digital Cell Phone inc should increase it is production at these 3 months .**
