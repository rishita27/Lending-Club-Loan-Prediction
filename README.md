# Lending-Club-Loan-Prediction
Lending Club is a US peer-to-peer lending company, headquartered in San Francisco, California. It was the first peer-
to-peer lender to register its offerings as securities with the Securities and Exchange Commission (SEC), and to offer loan trading on a secondary market. Lending Club is the world's largest peer-to-peer lending platform.

The dataset that has been taken is lending_club_loan.csv from kaggle.

Steps that have been implemented in this project

1. Exploratory Data Analysis

Plotted a countplot for the loan_status column. It is simply a visualization with pandas.

A histogram for the same i.e., for loan_status column. Histogram can only be plotted between two numerical columns. Hence, I will label encode the loan_status column first which will assign 0 to charged off and 1 to fully paid.

I will find the correlation between the continuous feature variables. Correlation tells us the degree to which variables that are present in our dataset are dependent upon each other. We can use df.corr() which will give us the data for the correlation. With the help of corr() we can find the pairwise correlation of all columns in a dataframe. Here is the correlation between all the continuous numeric variable.

Now, I have visualized the above task using a heatmap. Heatmap is again a data visualization technique which lets us see the variation of a relation. The value of correlation can take any value ranging from -1 to 1. A graphical representation of correlation heatmap which represents correlation between the continuous feature variables of the dataframe.

3. 

