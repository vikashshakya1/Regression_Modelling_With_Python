Heart attacks, also known as myocardial infarctions, are a leading cause of morbidity and mortality worldwide. Early prediction and intervention can significantly improve patient outcomes and reduce the burden on healthcare systems. Multiple regression analysis is a powerful statistical tool that can help identify and quantify the relationships between various risk factors and the likelihood of a heart attack. In the context of heart attack prediction, the dependent variable could be the occurrence of a heart attack, while the independent variables could include a range of clinical and demographic factors such as age, cholesterol levels, blood pressure, smoking status, and physical activity.

Here, I have built a LinearRegression model with the training and testing data.
![image](https://github.com/vikashshakya1/Regression_Modelling_With_Python/assets/142865487/456d8101-8183-4336-b699-dab10f773fa2)

**The scatter plot shown in the image visualizes the relationship between the actual values and the predicted values obtained from a model.
The blue dots represent individual data points, where each dot's x-coordinate corresponds to the actual value, and its y-coordinate corresponds to the predicted value for that particular data point.
Additionally, a red diagonal line is plotted, which represents the perfect prediction line. If all the predicted values were equal to the actual values, all the data points would fall exactly on this line.
**
![image](https://github.com/vikashshakya1/Regression_Modelling_With_Python/assets/142865487/154264a8-239c-4825-ac78-742e116cfda7)

**A Q-Q (Quantile-Quantile)** plot is a graphical tool to help assess if a dataset follows a particular theoretical distribution, most commonly the normal distribution. It plots the quantiles of your data against the quantiles of the specified theoretical distribution. If the points lie approximately along a straight line, the dataset is likely to follow the theoretical distribution.
![image](https://github.com/vikashshakya1/Regression_Modelling_With_Python/assets/142865487/dfe6f131-212e-44d0-b023-b2c719a5bfc1)

**Linearity**
The code generates scatter plots to visualize the relationship between each feature and the target variable in the dataset. It begins by defining the independent variables “X” and the dependent variable “y” from the dataset. Then, it iterates through each feature, creating a scatter plot with the target variable. Each subplot represents a feature, with feature values on the x-axis and target variable values on the y-axis. The title of each subplot indicates which feature is being plotted against the target variable. Finally, the layout is adjusted to prevent overlap between subplots, and the scatter plots are displayed.
![image](https://github.com/vikashshakya1/Regression_Modelling_With_Python/assets/142865487/e93723b4-e827-4f82-8a3f-357112f32753)

**MultiCollinearity**
Multicollinearity arises when independent variables in a regression model are highly correlated, leading to various challenges in estimation and interpretation. These challenges include unstable estimates, difficulties in interpretation, inflated standard errors, misleading variable importance, and reduced precision.
![image](https://github.com/vikashshakya1/Regression_Modelling_With_Python/assets/142865487/eb632f94-1395-4a59-aef3-1159a2781817)


**The Shapiro-Wilk test** is a statistical test used to assess whether a given sample of data follows a normal distribution. It is particularly useful when the sample size is small (typically less than 50-200 observations).
![image](https://github.com/vikashshakya1/Regression_Modelling_With_Python/assets/142865487/17fb0018-29b5-45ad-8b3a-75c45512b3e9)



