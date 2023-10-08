# Stock Price Forecasting

This study's objective is to conduct a descriptive and predictive analysis of Apple Inc.'s stock closing price to better understand the company's performance. By doing time series forecasting and regression analysis, the changes in the stock's closing price are studied using techniques such as moving average (MA), shifts/lags, correlation, root-mean-square error (RMSE), R-squared, p-value, Mean, Median, Mode and standard deviation. These tools are used in conjunction with one another. The purpose of this research is to determine the changes in stock price that occurred for Apple from the 1st of June 2017 through the 15th of September 2022. Based on these prices, which are then studied and examined with the help of the aforementioned indicators, conclusions are reached about the general trend of price swings as well as whether the stock should be purchased or sold in the near future.

# Data Collection Process

The data that was used for the study, which covers the time period beginning June 1, 2017, and ending September 15, 2022, was derived from the observations supplied by Apple's official website and by Yahoo Finance. Excel is used in the analysis process. The time series forecasting and regression analysis that was performed for predictive analysis, the development of the d.log close that was produced by the 
data analysis and the calculation of the mean, median, mode, and standard deviation for the data that was studied using the descriptive statistics method were all carried out during the aforementioned period. Additionally, histograms, scatter plots, and line graphs are representations of the data visualization in this draft.

# Techniques used for the Analysis
Descriptive Statistics
   Central Tendency - Mean, Median & Mode
   Standard deviation
   Skewness
Predictive Analysis
   Time Series Forecasting
   Regression Analysis
   R Square
   Residual
   RMSE (Root mean squared error)
   Moving Averages (MA)
   Lags/Shifts
   Correlation
# Descriptive Statistics for Apple’s stock closing price
In this section of the analysis, we have utilized the closing price of Apple’s stock for the duration of June 1st, 2017, through September 15, 2022. Firstly, we approached finding the log value for the closing price and further proceeded with the data analysis tool to produce the histogram graph. We have transformed the stock’s closing value into a log form. As we can see in the data, the data are in a log-normal distribution, meaning the actual value never takes on a negative value and is always right-skewed; hence, the actual value or the log-normal distribution is always positive. So, to carry out the statistics, we have transformed the actual values into log form in order to analyze the descriptive statistics in a more microscopic way.
<img width="475" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/b9c2f905-81c8-4568-84a8-47107087b9de">
<img width="257" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/f0b2bbfc-c5a9-4707-a8af-8938f3fc924e">

From the above figures, the histogram is slightly asymmetrical with a skewness of 0.318978. Hence, we can conclude the histogram is slightly right-skewed. Where the mean is -0.00045, the median is -0.0005, and the mode is 0.

# Predictive Analysis for Apple’s stock closing price
In this approach, we have performed the linear regression model on Apple’s closing stock price for the duration of the 1st of June 2017 through the 15th of September 2022, keeping the date as order. In 
In addition to this, R-square and RMSE values were determined, and the trend line was plotted against the actual values. The below figures will justify the above-mentioned queries.
<img width="221" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/ea0ca427-677f-48ac-822b-6222efcad3e0">
<img width="479" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/114f4381-f10c-46fc-af5c-df04fc9d9489">
<img width="485" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/40547b8b-55d0-41ce-83e1-15ca14abd819">

As per the observations above, the R-square is 0.88429185, and the RMSE value for the model is 15.95829331. As R-Square approaches 1, we may infer that the fit is better, and the closer it gets to 1, the more accurately the regression equation forecasts the dependent variable. In this case, we see the RMSE value is greater than 1. So, determining Normalized RMSE or NRMSE in this case –
Normalized RMSE = RMSE/(Max Value - Min Value)
 = 15.95/(182.00 - 35.54)
 = 15.95/146.46
 NRMSE = 0.10

Hence, after normalizing the RMSE value = 0.10, we can clearly confirm the model is more accurate in forecasting the dependent variable. Now, we have considered a case of Moving Averages for 5 days, 10 days and 15 days and performed a pairwise correlation analysis among all three moving averages and the stock’s closing price, which is shown below in the figure
<img width="331" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/0a7a0572-86eb-4180-9e6e-c1c888bb43c4">
From the above observations in the figure, we can clearly conclude that the relationship between the stock’s closing price and the moving averages for 5, 10, and 15 days, respectively, is close to +1; hence, a positive relationship can be proved. Furthermore, keeping the stock’s closing value as the actual value, we have tried to find the lags/shifts and followed the same process as above to determine the pairwise correlation among the 10 lags/shifts against the stock closing price as shown in the figure below.

<img width="255" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/b25bd84e-d1d7-46da-9eef-aff0fc86579d">
<img width="481" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/029217a4-3d75-420d-9ad2-aa2a89011de3">
Again, from the above observation, the results are quite similar to the operation performed with moving averages, i.e., the relationship between the 10 lags to the stock’s closing price is close to +1, and a positive relationship is confirmed. In contrast to the above analysis of the correlation between moving averages and lags and the stock’s closing price, we have tried to determine the best possible combination of the parameters, combining the moving averages and lags, performing the regression analysis, and determining the R-squared and RMSE values for the best-found model. Keeping this in mind, to avoid overfitting the model by considering 3 moving averages and 10 lags, we attempted to carry out an analysis in phases by maintaining a close eye on the p-value and eliminating the elements that had a high value for that statistic. This allowed us to do the study more effectively. After repeatedly repeating the same procedures, we ultimately came to a point where it was observed that the p-values were low or inconsequential, which assisted in avoiding overfitting the model.
<img width="477" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/1cebaf0e-487e-41e9-b894-bfdca698b045">
<img width="459" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/028dab79-bcbb-42bf-bb89-d25cc1f61aef">
<img width="482" alt="image" src="https://github.com/Rajdeep096/Stock-Price-Forecasting/assets/147287417/8a1180aa-8934-444e-83ef-0abb6636d096">

From the above figures, we determine the R squared = 0.998189 and the RMSE = 1.993589, and the Line graph figure is plotted after the analysis is done as per the above figure
Now, as per the multiple linear regression equation, y = mx1 + mx2+ mx3+ b, where,
Y = the dependent variable of the regression
M = slope of the regression
x1 = first independent variable of the regression
x2 = second independent variable of the regression
x3 = third independent variable of the regression
b = constant
We can determine our equation for the model as per the above figure: y = 0.9368*Lag1 + 0.0435*Lag2 + 0.0526*Lag4 - 0.0699*Lag6 + 0.0879*Lag7 - 0.1249*Lag8 + 0.07328*Lag9 + 0.15071
Using the above model, which we have produced after checking the correlations between Moving averages, Lags/Shifts, and a step-wise elimination of a higher p-value, we can determine that the model is 
accurate to the actual value, which is the stock price of Apple’s closing value. The figure above is the line chart that graphically represents the actual data vs. our predicted data as the model we have produced above. Hence, after the regression analysis, the R-squared value obtained is 0.998189, which is also aligned with the aforementioned facts. According to our problem statement, we have aimed to find a forecasting model that will determine the future values of Apple’s stock based on its closing value, and any investor, stakeholder, or trader can use the above models to predict whether an individual will trade or invest in this stock or not.

# Conclusion
In this report, we have used Apple’s stock closing price data to predict a forecasting model that will help any stakeholder determine the future value of the share price. We have discussed the data 
collection process and the various tools and techniques that were taught in class. This report also concludes on the descriptive statistics, which involve mean, median, mode, skewness, etc., and covers the predictive analysis section, where linear regression was performed by considering the R2 value and RMSE in contrast to other regression parameters like the concepts related to moving averages, lags/shifts, and correlation. For data visualization, we have used linear charts and the histogram available in MS Excel. Lastly, by using the above methods, we concluded a model which helps in forecasting the future values of Apple Stock’s closing price, which will help investors make a decision to invest in the stock.











