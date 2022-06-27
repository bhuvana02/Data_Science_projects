# Data_Science_Learning
## Index

•	[Python](https://github.com/bhuvana02/Data_Science_Learning/tree/main/python)
1.	[Python_practice_programs_1.ipynb](https://github.com/bhuvana02/Data_Science_Learning/blob/main/python/Python_practice_programs_1.ipynb)
2.	[python_practice_programs2.ipynb](https://github.com/bhuvana02/Data_Science_Learning/blob/main/python/python_practice_programs2.ipynb)
3.	[hanoi_using_recursion.ipynb](https://github.com/bhuvana02/Data_Science_Learning/blob/main/python/hanoi_using_recursion.ipynb)

 • [Data analysis](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Data%20analysis)
 
 1. [	Data_analysis_practice_on_loan_data.ipynb](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Data%20analysis/Data_analysis_practice_on_loan_data)
 2. [Data_analysis_practice_on_telecom_data.ipynb](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Data%20analysis/Data_analysis_practice_on_telecom_data)
 3. [Regression_MAE.ipynb](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Data%20analysis/Regression_MAE)
 


•	[Machine_learning_algorithms](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Machine_learning_algorithms)
1.	[Linear Regression .ipynb](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Machine_learning_algorithms/Linear%20Regression)

•	[Hackathons](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Hackathons)
1.	[User_video_engagement_score (JOB_HACKATHON)](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Hackathons/User_video_engagement_score%20(JOB_HACKATHON))
2.	[customer_churn_prediction](https://github.com/bhuvana02/Data_Science_Learning/tree/main/Hackathons/customer_churn_prediction)

# Approach:([customer_churn_prediction)
 Churn Prediction is Binary Classification Problem.

# Data Modelling and Model Selection is done in Four Steps :

 • Data-Preprocessing
 
 • Data Visualization
 
 • Feature Engineering
 
 • Machine Learning Algorithm (Modelling Part)



# Data Preprocessing:

  Perform data pre-processing wherever needed
  
 • Check for Missing Values and Imputing it.
    
 • Removing Duplicate Values.
    
 • Checking If there is Not Null Values and Dropping or Deleting it.
    
 • Check for the Data Types of DataFrame.
 
 • Also, Check for Age column if there is any anomaly present like if Age > 100 or Age <0. So, there is no anomaly found in Dataset.
 
 • Identifying Numerical and Categorical Column in the dataset.
 
 • And Dividing dataset into Categorical and Numerical Columns for Visualization.

# Data Visualization:

   • Derive some relevant insights out of the given data using different approaches
     (Such as using Seaborn/Matplotlib.)
     
   • Detecting Outliers
   
   • Relevant Insights
   
   • For Numerical columns plotting boxplot to Detect outlier in the dataset.
   
   • For Categorical columns plotting Barplot to detect which Column is more effecting theTarget Column (Is_Churn).
   
   • Descriptive Analysis of Dataset


# Feature Engineering:

   • In the DataSet, the Classes are Imbalance (it means the Class ‘0’ is Majority Class and
Class ‘1’ is Minority Class). So to Deal with Imbalance Classes Problem the Sampling
has to be done. To balance these Imbalance Classes used Resampling (Over Sampling)
to match the Count of Majority Class. After Resampling the Majority and Minority
Classes are approximately equal.

• In the dataset there are two types of Columns:

## Categorical Columns
  • For Categorical Columns, applied LabelEncoder for Two Class Columns and for more
than two applied OrdinalEncoder (Here OrdinalEncoder because the Categorical
Columns has the data in a Order Form Like Income Column, Product Holdings etc).

## Numerical Columns

  • After Encoding Categorical Columns, check for MultiCollinearity. So the Age has VIF value > 5 which is Highly MultiCollinear.
  
  • And Also the Balance Column Contains Outliers. So to Overcome from these two aboveColumn the data is Normalize using the MinMaxScaler(Numerical Columns: Age,Balance). After Scaling Data the MutliCollinearity has low Values
  
  • Checking for the Correlation by Plotting heatmap and removing the columns which
are highly Correlated.

  • Applying Statistical Techniques to Find Significant Columns. Here used Generalized
Linear Model Regression or Ordinary least-squares model to find the relationship
between Dependent and Independent Columns or Variables. The Columns which has
P-value > 0.05(Significance Value) are not Significant for the Target (Is_Churn) or not
contribute for the Target Column.

• Take only the relevant attributes for building the Models.


# Model Selection :

• Build Model Using Logistic Regression, Gaussian Naïve Bayes, Decision Tree Classifier,
Random Forest Classifier, XGB Classifier, Support Vector Machine, KNN individually

• Performed Model Selection according to the Model which perform best Prediction
Score and with Best F1 (Macro) Evaluation Metrics.

• And for Model Selection, Selecting the Model with High Prediction Score on Test Data
which is Gaussian Naïve Bayes have Prediction Score of 0.6190472511



From Above All Different Model, Gaussian Naïve Bayes and Logistic Regression are good
Fitted Model for Binary Classification. Gaussian Naïve Bayes and Logistics Regression both
the Model has very close or approximately Equal Prediction Score on Test Data but Gaussian
Naïve Bayes gives best Prediction Score. Gaussian Naïve Bayes is predicted good for Test
Data because most of the Column follows Normal Distribution.
Gaussian Naïve Prediction Score: 0.6190472511
Logistic Regression Prediction Score: 0.606211702511114

