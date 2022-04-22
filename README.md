# Bank Personal Loan Analisys with Python
## Project overview
* We need to know which factors influence to give a loan
* We also need to look for any opportunity to increase the bank's assets
* It was found that apart from income, family size is an important factor
* The libraries used were pandas, numpy, matplotlib, seaborn and scipy
* You can access the Jupiter Notebook [HERE](https://github.com/victort9/Bank_Loan_Project/blob/main/Files/Bank_Personal_Loan_Analysis.ipynb)

## Objective
### Questions that will drive the analysis
Central question:

**What is the most important factor to give a personal loan?**

Other questions:

* What is the relationship between education and personal loan?
* What is the distribution of the client population?
* What types of accounts and security do our clients have?
* What is the relationship between income and loans?
* What is the relationship between mortgage and loans?

## Data cleaning and data preparation

The file Bank_Personal_Loan_Data.csv contains data on 5000 customers, you can see the raw data [HERE](https://github.com/victort9/Bank_Loan_Project/blob/main/Files/Bank_Personal_Loan_Data.csv). 

The data include customer demographic information, like "age", "income"... the customer's relationship with the bank, like "mortgage", "securities account"... and the customer response to the last personal loan campaign "Personal Loan".

The activities performed were the following:

* "ID" has had to be removed because it is not related to the loan. 
* The "ZIP Code" has also been removed because we can judge the customers based on their area or location by looking the price of the houses in that area, but in this case we will use only the income.
* Elimination of negative values
* Exploration of the correlation of data and outliers: There is a strong correlation between age and experience

![](https://github.com/victort9/Bank_Loan_Project/blob/main/Images/Correlation_heatmap.png)


* Analysis of the distribution of the data: A large number of outliers were found in income

![](https://github.com/victort9/Bank_Loan_Project/blob/main/Images/Boxplot.png)


![](https://github.com/victort9/Bank_Loan_Project/blob/main/Images/histogram.png)


## Exploratory Data Analysis
The EDA was done with the target questions in mind "What is the most important factor to give a personal loan?". Several conclusions were obtained which will be presented below.

* Distribution of client education: The most of clients are undergraduates but it appears that education does not have a direct relationship with personal loan.


![](https://github.com/victort9/Bank_Loan_Project/blob/main/Images/Pie_education.png)

![](https://github.com/victort9/Bank_Loan_Project/blob/main/Images/Boxplot_persn_loan.png)


* Analysis of client account type: The vast majority of clients do not have a security or credit account. It could generate some extra assets for the bank if we find a way to encourage them to have one.


![](https://github.com/victort9/Bank_Loan_Project/blob/main/Images/Pie_account_type.png)


* Personal loan in relation to other factors: It seems that the most important factor for a loan is income, no surprise there. Another really important factor is the number of relatives in the family.


![](https://github.com/victort9/Bank_Loan_Project/blob/main/Images/Income_persn_loan.png)


## Conclusions
* The most influential values are income and family size.
* The least influential values are age and experience.
* It is advisable to encourage customers to create a credit account and security.
* You can access the code [HERE](https://github.com/victort9/Bank_Loan_Project/blob/main/Files/Bank_Personal_Loan_Analysis.ipynb).
