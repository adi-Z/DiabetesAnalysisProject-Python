Project - Diabetes Analysis
----------------------------
Overview
This project focuses on conducting an exploratory data analysis (EDA) to gain insights into the factors associated with diabetes in the Pima tribe. Leveraging statistical analysis and data visualization, the project aims to understand the key factors contributing to diabetes within a specific context.

Additionally, the project involves building predictive models to forecast future outcomes related to diabetes. Using machine learning techniques, the aim is to develop accurate models that can assist in predicting the likelihood of diabetes based on various features.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Context
A few years ago, research on the Pima tribe (Pima Indians) revealed a high susceptibility to diabetes among the female members, particularly at an early age. This project aims to explore and understand different factors associated with diabetes within this population.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Data Source
The dataset used in this analysis is sourced from diabetes.csv

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Data Dictionary
Pregnancies:  Number of times pregnant
Glucose:  Plasma glucose concentration over 2 hours in an oral glucose tolerance test
BloodPressure:  Diastolic blood pressure (mm Hg)
SkinThickness:  Triceps skin fold thickness (mm)
Insulin:  2-Hour serum insulin (mu U/ml)
BMI:  Body mass index (weight in kg/(height in m)^2)
DiabetesPedigreeFunction:  A function scoring the likelihood of diabetes based on family history.
Age:  Age in years
Outcome:  Class variable (0: person is not diabetic or 1: person is diabetic)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Tools and Libraries Used
•	Python
•	NumPy
•	Pandas
•	Seaborn
•	Matplotlib
•	Scikit-learn

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Exploratory Data Analysis (EDA)
The project involves thorough EDA using various visualizations and statistical measures to uncover insights into the factors associated with diabetes in the Pima tribe.

Key Findings
Distribution of Blood Pressure: 
•	Visual representation of the distribution of blood pressure using a seaborn distplot.
Observation - The distribution of the variable BloodPressure can be considered normal because it is bell-shaped and symmetrical. The plot appears to have an outlier on the left side. 

BMI Statistics: 
•	Mean, median, and mode of BMI calculated.
Observation - The individual exhibiting the highest glucose level possesses a BMI index of 42.9. The average value (mean) for the BMI variable is 32.7, with a median of 32.8. Additionally, the mode for BMI is recorded at 32.

Glucose Comparison: 
•	Number of women with glucose higher than the mean glucose.
Observation - 449 women exhibit glucose levels higher than the mean.

 Pairplot and Scatterplot: 
•	Visualization of relationships between Glucose, SkinThickness, and DiabetesPedigreeFunction using pairplot.
•	Scatterplot of Glucose against Insulin.
Observation (Pairplot) - Individuals with lower glucose levels and a lower diabetes pedigree function are more likely to avoid a diabetes diagnosis. Conversely, there is no evident correlation between SkinThickness, DiabetesPedigreeFunction, and the ultimate outcome of diabetes.

Observation (Scatterplot) - Insulin and glucose levels exhibit a direct correlation, where an increase in glucose levels corresponds to a concurrent increase in insulin levels.

Age Boxplot: 
•	Boxplot representing the distribution of ages.
Observation - The Age variable exhibits the presence of outliers.

Correlation Matrix: 
•	Heatmap depicting the correlation matrix of the features.
Observation - Variables "Age" and "Pregnancy" exhibit a moderately positive correlation.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Model Building
Two classification models were employed:
Logistic Regression
•	Model Accuracy on Train Set: __76%_
•	Model Accuracy on Test Set: _75%___
•	Confusion Matrix: _array([[60,15] , [22,53]])___

Random Forest Classifier
•	Model Accuracy on Train Set: _82%___
•	Model Accuracy on Test Set: _79%___
•	Confusion Matrix: __ array([[56,19] , [13,62]])_____

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Conclusion
The project provides valuable insights into the factors associated with diabetes in the Pima tribe. The analysis includes visualizations, statistical measures, and the implementation of machine learning models for prediction.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

How to Use
1. Ensure you have the required libraries installed (NumPy, Pandas, Seaborn, Matplotlib, Scikit-learn).
2. Clone the repository: `git clone [https://github.com/adi-Z/DiabetesAnalysisProject-Python]`.
3. Run the Jupyter notebook or Python script for detailed exploration and analysis.
