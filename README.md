**"A Statistical Approach to Heart Attack Prediction: Multiple Regression Modelling"**
1.Introduction:
Heart attacks, also known as myocardial infarctions, are a leading cause of morbidity and mortality worldwide. Early prediction and intervention can significantly improve patient outcomes and reduce the burden on healthcare systems. Multiple regression analysis is a powerful statistical tool that can help identify and quantify the relationships between various risk factors and the likelihood of a heart attack. In the context of heart attack prediction, the dependent variable could be the occurrence of a heart attack, while the independent variables could include a range of clinical and demographic factors such as age, cholesterol levels, blood pressure, smoking status, and physical activity.

2.Dataset Description and Course:
The dataset used in this analysis is related to heart attacks and contains various clinical and demographic factors that may influence the risk of a heart attack. This dataset provides a comprehensive set of features that can be used to develop a predictive model for heart attack risk.
Here are the key details about the dataset:
Source: The dataset is a collection of medical data from patients, including both those who have experienced heart attacks and those who have not. It is commonly used in the medical field for research and predictive modelling.
Observations: The dataset contains records for a number of patients (e.g., 700 observations).
Features: The dataset includes the following features:
Age: Age of the patient.
Sex: Gender of the patient (1 = male, 0 = female).
CP: Chest pain type (1 = typical angina, 2 = atypical angina, 3 = non-anginal pain, 4 = asymptomatic).
Trestbps: Resting blood pressure (in mm Hg).
Chol: Serum cholesterol in mg/dl.
Fbs: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false).
Restecg: Resting electrocardiographic results (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy by Estes' criteria).
Thalach: Maximum heart rate achieved.
Exang: Exercise-induced angina (1 = yes, 0 = no).
Oldpeak: ST depression induced by exercise relative to rest.
Slope: The slope of the peak exercise ST segment (1 = upsloping, 2 = flat, 3 = downsloping).
Ca: Number of major vessels (0-3) colored by fluoroscopy.
Thal: Thalassemia (3 = normal, 6 = fixed defect, 7 = reversible defect).
Target: Diagnosis of heart disease (0 = no disease, 1 = disease).
This dataset captures a wide range of potential predictors for heart attacks, making it suitable for multiple regression analysis.
Course of Analysis:
1.	Data Preprocessing
	Loading the Data
	Handling Missing Values
	Feature Selection
2.	Exploratory Data Analysis (EDA)
	Descriptive Statistics
	Correlation Analysis
	Visualization
3.	Data Splitting
4.	Model Building
5.	Model Evaluation
6.	Interpretation of Results
7.	Conclusion
3.AIM/Objective: 
The primary aim of this analysis is to develop a robust multiple regression model to predict the risk of heart attacks based on various clinical and demographic factors. By leveraging the dataset that includes comprehensive patient information, the objectives of this analysis are as follows:
•	Identify Key Risk Factors: Determine which clinical and demographic factors significantly contribute to the risk of a heart attack. This involves analysing the relationships between potential predictors (e.g., age, cholesterol levels, blood pressure) and the target outcome (presence of heart disease).
•	Build a Predictive Model: Construct a multiple regression model that can accurately predict the likelihood of a heart attack. This involves training the model on a portion of the dataset and validating its performance on the remaining data.
•	Evaluate Model Performance: Assess the adequacy and accuracy of the regression model using performance metrics such as the R² score, Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). These metrics will help in understanding how well the model explains the variability in the target variable and how accurately it predicts heart attack risk.
•	Interpret Model Coefficients: Analyse the regression coefficients to understand the impact of each predictor on the risk of a heart attack. This interpretation will provide insights into which factors have the most significant influence and could inform preventive healthcare strategies.
•	Provide Insights for Preventive Measures: Based on the findings, offer recommendations for healthcare practitioners to identify high-risk individuals and take preventive measures. Understanding the key risk factors and their impact can help in developing targeted interventions to reduce the incidence of heart attacks.
Specific Objectives:
•	Data Preprocessing
•	Exploratory Data Analysis (EDA)
•	Model Training and Validation
•	Residual Analysis
•	Visualization of Results
By achieving these objectives, the analysis aims to provide a comprehensive understanding of heart attack risk factors and develop a predictive tool that can assist in early detection and intervention, ultimately contributing to better cardiovascular health outcomes.
4. Analysis:
 
Here, I have built a LinearRegression model with the training and testing data.
 
I have also calculated the Root Mean Square Error and  R^2 Score which tells us that our model is good and with good accuracy.
 
The scatter plot shown in the image visualizes the relationship between the actual values and the predicted values obtained from a model.
The blue dots represent individual data points, where each dot's x-coordinate corresponds to the actual value, and its y-coordinate corresponds to the predicted value for that particular data point.
Additionally, a red diagonal line is plotted, which represents the perfect prediction line. If all the predicted values were equal to the actual values, all the data points would fall exactly on this line.
 
Calculating and analysing the coefficients of a linear regression model is crucial for several reasons:
1.	Interpretation of the Model
2.	Understanding Feature Importance
3.	Model Diagnostics
4.	Decision Making
 
The graph shown in the image displays the coefficients of different features or variables used in a linear or logistic regression model. The x-axis represents the coefficient values, while the y-axis lists the names of the features or variables.
Each horizontal bar corresponds to a feature, and its length represents the magnitude and direction (positive or negative) of its coefficient in the model. The coefficients indicate the relative importance and impact of each feature on the target variable or outcome being predicted by the model.
Features with positive coefficients (bars extending to the right) have a positive relationship with the target variable, meaning that as their values increase, the predicted value of the target variable also tends to increase. Conversely, features with negative coefficients (bars extending to the left) have a negative relationship with the target variable, indicating that as their values increase, the predicted value of the target variable decreases.
Q-Q plot:
A Q-Q (Quantile-Quantile) plot is a graphical tool to help assess if a dataset follows a particular theoretical distribution, most commonly the normal distribution. It plots the quantiles of your data against the quantiles of the specified theoretical distribution. If the points lie approximately along a straight line, the dataset is likely to follow the theoretical distribution.
 
This code segment performs several statistical analyses on the residuals of a model:

1.Residuals are calculated by subtracting the predicted values (“y_pred”) from the actual values (“y_test”).
2. A Q-Q (quantile-quantile) plot is created using Matplotlib. This plot compares the distribution of the residuals to a normal distribution. It helps assess if the residuals follow a normal distribution, which is an assumption of many statistical models.
 
In the given plot, the blue dots represent the observed quantiles plotted against the theoretical quantiles. The observed quantiles generally follow a linear pattern, but there are some deviations from the reference line, particularly in the tails (extreme values) of the distribution. The Q-Q plot is useful for detecting departures from the assumed distribution. If the points deviate substantially from the reference line, it may indicate that the data does not follow the assumed distribution or that there are outliers or other anomalies in the data.
 
The code generates scatter plots to visualize the relationship between each feature and the target variable in the dataset. It begins by defining the independent variables “X” and the dependent variable “y” from the dataset. Then, it iterates through each feature, creating a scatter plot with the target variable. Each subplot represents a feature, with feature values on the x-axis and target variable values on the y-axis. The title of each subplot indicates which feature is being plotted against the target variable. Finally, the layout is adjusted to prevent overlap between subplots, and the scatter plots are displayed.
 
The image shows multiple scatter plots, each visualizing the relationship between a specific feature or variable (shown on the x-axis) and the target variable (shown on the y-axis) of a dataset. These scatter plots are useful for exploring potential correlations and patterns between the independent variables and the dependent variable in a regression or classification problem.
Each subplot represents a scatter plot between one feature and the target variable. The points are spread across the plot, allowing you to visually examine the distribution of the data points and identify potential relationships or trends.
For example, in the scatter plot titled "Scatter Plot: age vs target", the x-axis represents the age feature, and the y-axis represents the target variable. The scattered points show how the target variable values vary with respect to different age values.
 
This code conducts linear regression analysis on a dataset using the `stats models` library in Python. Here's what each step accomplishes:
1.Adding a Constant Term: By adding a constant term using `sm.add_constant ()`, we ensure that the linear regression model includes an intercept term. This is important because it allows the regression line to intersect the y-axis at a specific point rather than being forced to pass through the origin
2. Fitting the Linear Regression Model: We create an ordinary least squares (OLS) regression model using `sm.OLS()`. This model takes the dependent variable (`y`) and the independent variables (`X`) as arguments. The `fit()` method then fits the model to the data, estimating the coefficients for the intercept and each independent variable.
3.Printing the Model Summary: The `summary()` method prints out a comprehensive summary of the fitted regression model. This summary includes information such as coefficients, standard errors, t-values, p-values, and goodness-of-fit measures like R-squared and adjusted R-squared. It provides insights into the relationship between the independent variables and the dependent variable, as well as the overall performance of the model.
In essence, this code segment performs linear regression analysis to understand the linear relationship between the independent variables and the dependent variable in the dataset.

 
These are all the coefficient of all the features that are in our dataset and OLS regression results.

Residuals:
Residuals, in the context of linear regression analysis, refer to the differences between the observed values of the dependent variable and the values predicted by the regression model.
Residuals are essential in assessing the quality of a regression model. Ideally, in a well-fitted model, the residuals should be small and evenly distributed around zero. If the residuals exhibit patterns or have large deviations from zero, it indicates that the model may not adequately capture the relationship between the independent and dependent variables.
This code segment generates a residual plot to evaluate the linearity assumption of a linear regression model. It calculates the fitted values and residuals from the model, then creates a scatter plot with fitted values on the x-axis and residuals on the y-axis. A horizontal dashed line at y=0 is added for reference. The plot allows visual inspection of whether the residuals are evenly distributed around zero, which is indicative of a well-fitted linear regression model.
 
 
Pearson Coefficient:
The Pearson correlation coefficient, often denoted as 𝑟, is a statistic that measures the linear relationship between two continuous variables. It ranges from -1 to 1, where:
•	R=1 indicates a perfect positive linear relationship,
•	R= −1 indicates a perfect negative linear relationship,
•	R=0 indicates no linear relationship between the variables.
The Pearson correlation coefficient measures both the strength and direction of the linear relationship between two variables. A value closer to 1 or -1 indicates a stronger linear relationship, while a value closer to 0 indicates weaker or no linear relationship.
This code calculates the Pearson correlation coefficient between each feature in the dataset (X) and the target variable (y). Here's a summary:
Importing Necessary Libraries: The code imports NumPy as np, assuming it's needed for numerical operations.
Correlation Calculation: It initializes an empty list correlation_coefficients to store the correlation coefficients. Then, it iterates through each feature in X.columns and calculates the Pearson correlation coefficient between that feature and the target variable y using np.corrcoef(). The correlation coefficient is then appended to the correlation_coefficients list.

Printing Correlation Coefficients: Finally, it iterates through the columns of X and the corresponding correlation coefficients stored in correlation_coefficients, printing out each feature's name along with its calculated correlation coefficient.
In summary, this code segment computes and prints the Pearson correlation coefficient for each feature in the dataset with respect to the target variable. It helps to understand the linear relationship between each feature and the target variable.
 

Multicollinearity:
Multicollinearity arises when independent variables in a regression model are highly correlated, leading to various challenges in estimation and interpretation. These challenges include unstable estimates, difficulties in interpretation, inflated standard errors, misleading variable importance, and reduced precision. Detecting multicollinearity is crucial before interpreting regression results, and common methods for detection include variance inflation factors (VIFs), correlation matrices, and condition indices. Strategies for addressing multicollinearity involve removing redundant variables, combining correlated variables, or using regularization techniques such as ridge regression. Understanding and managing multicollinearity are vital for accurate and reliable regression analysis.
 
This code segment aims to assess multicollinearity among the independent variables in a regression model using Variance Inflation Factors (VIFs). Here's a summary:
1. **Initialization of DataFrame**: A DataFrame named `vif_data` is initialized to store the feature names and their corresponding VIF values.
2. **Computation of VIFs**: For each feature in the dataset `X`, the VIF is calculated using the `variance_inflation_factor` function from the `statsmodels.stats.outliers_influence` module. This function takes the design matrix (in this case, `X.values`) and the index of the feature as arguments.
•	VIF:  The Variance Inflation Factor (VIF) is a measure used to assess multicollinearity in a regression analysis. It quantifies how much the variance of the estimated regression coefficients is inflated due to multicollinearity among the independent variables.
3. **Displaying Results**: The calculated VIF values are then printed alongside their corresponding feature names using the `print()` function.
Overall, this code computes and displays the VIF values for each feature, providing insights into the degree of multicollinearity among the independent variables in the regression model. VIF values above a certain threshold (often 5 or 10) indicate multicollinearity, suggesting the need for further investigation or remedial actions.
The Shapiro-Wilk test:
The Shapiro-Wilk test is a statistical test used to assess whether a given sample of data follows a normal distribution. It is particularly useful when the sample size is small (typically less than 50-200 observations).
The Shapiro-Wilk test helps to assess the normality of data, which is an important assumption for many statistical analyses, including parametric tests like t-tests and ANOVA.
 
With a Durbin-Watson statistic of approximately 1.03, there's a slight indication of positive autocorrelation, implying that neighboring residuals may be positively correlated.
Breusch-Pagan test for homoscedasticity:
The Breusch-Pagan test is a statistical test used to assess whether the residuals of a regression model exhibit homoscedasticity, which means that the variance of the residuals is constant across all levels of the independent variables.
Action: If heteroscedasticity is detected, it may be necessary to address it by using robust standard errors or transforming the data appropriately to stabilize the variance across different levels of the independent variable.
Overall, the Breusch-Pagan test helps ensure the validity of regression analysis results by assessing whether the assumption of homoscedasticity is met.
Durbin-Watson Test : The Durbin-Watson test is a statistical test used to assess the presence of autocorrelation in the residuals of a regression model. Autocorrelation occurs when the errors (residuals) in a regression model are correlated with each other.
If the Durbin-Watson test statistic deviates significantly from 2 and the p-value associated with the test statistic is below a chosen significance level (e.g., 0.05), it provides evidence to reject the null hypothesis, indicating the presence of autocorrelation. In such cases, it may be necessary to address autocorrelation through model adjustments or transformation of the data.
 

Conclusion:
The multiple regression analysis was conducted to explore the relationship between various independent variables (age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal) and the target variable (indicating the presence or absence of heart disease).
The results of the regression analysis reveal that several independent variables have a statistically significant impact on the target variable. Notably, variables such as age, cp (chest pain type), thalach (maximum heart rate achieved), and oldpeak (ST depression induced by exercise relative to rest) demonstrate significant associations with the presence of heart disease.
Furthermore, the overall fit of the regression model was assessed using metrics such as R-squared. The R-squared value indicates that the model explains a significant proportion of the variance in the target variable, suggesting that the selected independent variables collectively contribute to predicting the presence or absence of heart disease.
In conclusion, the multiple regression analysis provides valuable insights into the factors influencing the occurrence of heart disease. The identified associations can potentially aid in risk assessment, diagnosis, and treatment planning for individuals at risk of cardiovascular conditions.
