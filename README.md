# Lending-Club-Loan-Prediction
Lending Club is a US peer-to-peer lending company, headquartered in San Francisco, California. It was the first peer-
to-peer lender to register its offerings as securities with the Securities and Exchange Commission (SEC), and to offer loan trading on a secondary market. Lending Club is the world's largest peer-to-peer lending platform.

The dataset that has been taken is lending_club_loan.csv from kaggle.
## ![Rishita Kotiyal header](https://github.com/rishita27/Lending-Club-Loan-Prediction/blob/master/Outputs/Info.png)

Steps that have been implemented in this project

## Exploratory Data Analysis

1. Plotted a countplot for the loan_status column. It is simply a visualization with pandas. A histogram for the same i.e., for loan_status column. Histogram can only be plotted between two numerical columns. Hence, I will label encode the loan_status column first which will assign 0 to charged off and 1 to fully paid. Some correlation between the continuous feature variables. Correlation tells us the degree to which variables that are present in our dataset are dependent upon each other. We can use df.corr() which will give us the data for the correlation. With the help of corr() we can find the pairwise correlation of all columns in a dataframe. Here is the correlation between all the continuous numeric variable. Heatmap is again a data visualization technique which lets us see the variation of a relation. The value of correlation can take any value ranging from -1 to 1. A graphical representation of correlation heatmap which represents correlation between the continuous feature variables of the dataframe.
## ![Rishita Kotiyal header](https://github.com/rishita27/Lending-Club-Loan-Prediction/blob/master/Outputs/image.png)
## ![Rishita Kotiyal header](https://github.com/rishita27/Lending-Club-Loan-Prediction/blob/master/Outputs/image-2.png)

2. To calculate the summary statistics a sub selection on these two columns is made first: df[["loan_amnt", "loan_status"]]. After that the groupby() method is applied on the loan_status column to make a group per category. The average loan amount for every loan status is calculated and returned.
## ![Rishita Kotiyal header](https://github.com/rishita27/Lending-Club-Loan-Prediction/blob/master/Outputs/Screenshot%202022-01-13%20at%206.40.25%20PM.png)

3. Analyzing the grade and subgrade column. Unique possible grades and subgrades are displayed. Displaying a countplot per subgrade. Countplot for the subgrade column. Sorted the column sub_grade so that we can get a clear countplot. Subgrades that don’t get paid back that often. There are two subgrades in the dataset that don't get paid often and those are F(1-5) and G(1-5). For these subgrades we will plot a countplot. Now we will create a new column that is loan_repaid and map the values of loan_status to it.
## ![Rishita Kotiyal header](https://github.com/rishita27/Lending-Club-Loan-Prediction/blob/master/Outputs/image-5.png)
## Data Preprocessing



