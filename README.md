# Assignment4

Name: Sriram Nalabolu, Student ID: 700740102

Video Link: https://youtu.be/tslxxASM-Lk

Explanation

Pandas

Question1:
1.	Importing pandas and then reading the data using pandas into df
2.	Printing the data loaded into df

Question2
1.	Displaying the statistics about the data loaded from the file using describe  

Question3
1.	Checking the data if the columns are having any null values using isnull().any(). It shows Boolean form of true or false. True for null values exist and false for null values doesn’t exist.
2.	Replacing the null values by the mean using fillna()
3.	Displaying the data again using isnull().any() and checking if they are replaced.

Question4
1.	Aggregating the two columns duration and calories with the computational values of minimum, maximum, count and mean using agg()

Question5
1.	Filtering the dataframe df using the & operator to select only the rows that has calories values between 500 and 1000 using slicing.

Question6
1.	Filtering the dataframe df using the & operator to select only the rows that has calories values greater than 500 and pulse values less than 100.

Question7
1.	Creating a new dataframe “df_modified” that contains all the columns from df except for “Maxpulse” column.
2.	Displaying the modified dataframe

Question8
1.	Deleting the Maxpulse column from the main dataframe df
2.	Displaying the dataframe after deleting the column.

Question9
1.	Checking the datatype of calories column by printing it
2.	Converting the datatype of calories column to int
3.	Checking the datatype of calories column by printing it after changing it to int datatype

Question10
1.	Creating a scatter plot using pandas i.e. using the data loaded into the dataframe df and printing it.

Titanic Dataset

Question1
1.	Importing pandas and creating the dataframe using pandas 
2.	Importing preprocessing using sklearn and then 
3.	Using a label encoder from preprocessing to convert categorical labels into numerical labels for the column sex
4.	Finding the correlation between ‘survived’ (target column) and ‘sex’ column for the Titanic use case in class after converting to numerical values.
5.	Dropping the categorical data columns from the dataframe created
6.	Creating corelation matrix for the dataframe after removing the categorical values
7.	Printing the matrix created.

Question1.a
As correlation results shows that males were strongly negatively correlated, and females were Strongly positively correlated with their survival. Males are inversely proportional, and females are directly proportional to their survival. So, we need this feature to analysis.

Question2
1.	Visualizing the data of titanic using df.corr().style.background_gradient()
2.	Importing seaborn and matplotlib.pyplot
3.	Using seaborn, heatmap and pyplot to visualize the data of titanic.

Question3
1.	Importing pandas, GaussianNB model, train_test_split, accuracy_score and SimpleImputer
2.	Reading the train dataset file and loading it into df
3.	Dividing the columns into features and target data
4.	Preprocessing the categorical values 
5.	Splitting the data into training and testing datasets using train_test_split
6.	Replacing missing values in the train data with mean
7.	Training the Naive Bayes model using the training data
8.	Making predictions on the test set using the model
9.	Calculating the accuracy of the model using accuracy_score
10.	Received an accuracy score of 77.65%

Glass Dataset - Naive Bayes

Question1
1.	Importing pandas, GaussianNB model, train_test_split
2.	Reading the train dataset file and loading it into df
3.	Dividing the data into x and y with y having target column and x having remaining features/columns
4.	Splitting the data into training and testing datasets

Question2
1.	Importing classification report using sklearn.metrics
2.	Training the naive bayes model that we imported using the train data
3.	Creating the predictions on test data
4.	Calculating the accuracy score and classification report
5.	Printing the accuracy score and classification report
6.	Received an accuracy score of 55.81%

Glass Dataset - SVM

Question1
1.	Importing pandas, train_test_split
2.	Reading the glass data into df
3.	Dividing the data into x and y with y having target column and x having remaining features/columns
4.	Splitting the data into training and testing datasets

Question2
1.	Importing Linear svm model, classification report using sklearn.metrics
2.	Training the linear svm model that we imported using the train data
3.	Creating the predictions on test data
4.	Calculating the accuracy score and classification report
5.	Printing the accuracy score and classification report
6.	Received the accuracy score of 51.16%

Do at least two visualizations to describe or show correlations in the Glass Dataset.
1.	Visualizing the data of glass using df.corr().style.background_gradient(). Df is the dataframe having the glass data
2.	Importing seaborn and matplotlib.pyplot
3.	Using seaborn, heatmap and pyplot to visualize the data of glass.

Which algorithm you got better accuracy? Can you justify why?
Naive Bayes and Support vector machine algorithms, naïve bayes got better accuracy than the SVM. Naive Bayes gives better results than SVM for this data set. we may get better results using SVM than naïve bayes when we work with another data set. In this glass data set, types of glass are independent predictors. When there are any independent predictors present in the data set naïve bayes perform better than other models.
