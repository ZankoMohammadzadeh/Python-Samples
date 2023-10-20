# Python-Samples

In this section, I will provide an overview of the types of Business Intelligence operations that can be effectively performed using Python libraries like Pandas(for data manipulation), Numpy(for numerical operations), matplotlib.pyplot (for data visualization), seaborn (for statistical data visualization), and scikit-learn's functions for model selection and metrics.

**Credit Scoring project** is a script that deals with credit scoring data. It performs various tasks related to data analysis, visualization, and the creation of a linear regression model. Here's a description of what each part of the code does:

  - ***Data Loading:***
It loads two datasets - 'Data_CreditScoring_Train.csv' and 'Data_CreditScoring_Test.csv' using pandas, with 'training_data' and 'testing_data' as the respective dataframes.

  - ***Data Exploration:***
The code prints the number of unique values in each column of the 'training_data' dataframe using training_data.nunique() and displays the first few rows of the training data using training_data.head().

  - ***Data Correlation:***
It calculates the correlation matrix for the numeric columns in the 'training_data' dataframe and generates a heatmap to visualize the correlations between features.

  - ***Data Visualization:***
Various visualizations are created, including histograms for selected metrics, scatter plots of 'AGE' against 'PAY_AMT1' and 'AGE' against 'BILL_AMT1', and a scatter plot comparing 'BILL_AMT1' and 'BILL_AMT2'.

  - ***Data Splitting:***
The training data is split into two subsets, 'train_data_separated' and 'test_data_separated', randomly based on a mask generated by 'np.random.rand'. The 80-20% split ratio is used.

  - ***Linear Regression Model:***
A linear regression model is created and trained on the 'train_data_separated' using 'BILL_AMT2' as the predictor and 'BILL_AMT3' as the target.
The coefficients and intercept of the linear regression model are printed and a scatter plot is generated to visualize the regression line.

  - ***Linear Regression Model Evaluation:***
The trained linear regression model is applied to the 'test_data_separated' to make predictions, and various regression metrics, including Mean Absolute Error, Mean Squared Error, and R-squared (R2) score, are printed.




