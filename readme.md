Loan Data Analysis:

Loan Data contained of 113937 rows and 81 columns such as ProsperScore, BorrowerAPR, AvailableBankcardCredit,Ishomeowner columns and many more.
This analysis was mainly to find the key factors driving Prosper Score and Borrower's APR.


Data Cleaning:

Missing values were present in few columns and needed to be treated.

Steps taken in Data cleaning process:
Choosing the columns necessary for analysis and copying into loan dataframe
Dropping CreditGrade column as it consists of high null percentage, imputing is not a best idea for this columns has almost 75% values are missing
Dropping rows having null values for ProsperScore as it's an important column for my analysis,shouldn't be biased because of imputation
11 is max score for ProsperScore which is incorrect, Retaining only rows having valid prosperscore from 1 to 10
'EmploymentStatusDuration' column consists of integar values, so imputing null values with median of that column
'AvailableBankcardCredit' column consists of integar values, so imputing null values with median of that column
'Occupation' column mode is given by 'Other', so imputing null values with it
'EmploymentStatus' column mode is given by 'Employed', so imputing null values with it
'DelinquenciesLast7Years' column consists of integar values, so imputing null values with median of that column
Imputing 'BorrowerAPR' null values with it's mean value

Summary of Visualization:

Most of the loan applicants have Occupation mentioned as 'Other', This includes the customers who had not specified what's their occupation and also those who didn't wish to specify the occupation
AvailableBankcardCredit maximum value is close to 500000 and most have the available credit around 10000 dollars.
Around 79 % of customers are employed, also there are columns such as Full-time, part-time which are separated from Employed. May be Employed column could have been omitted during data gathering process and right information should have been filled up in other columns.
Low number of customers are given 1 as the prosper score, most of them are given score between 4 and 8.
It can be seen that maximum number of customers have not missed their instalment, maximum of number of misses is close to 100.
Next maximum number of misses is 1, number of delinquencies is gradually reducing, which is a good sign as most customers tend to not default the loan.
Customers who are new to their job seem to apply for loan more frequently than others.
Most customers have borrowed loan at the annual percentage rate of 0.37, mean comes around 0.22
Most customers have borrowed loan at the rate of 0.33, mean comes around 0.19.
Close to 68% of customers have opted 36 month instalment scheme, next favourite is 60 months with 29% of customers opting for it
Most of the loan applicants have ongoing loans, assuring good cash flow for the bank if not defaulted.
Customers having own property seem to be applying for loan more than not being a owner customers though there is no much of a difference between their proportion.
Lower Borrower APR, means better prosper score
Borrower APR and Borrower Rate are positively correlated, it's obvious as Borrower APR is Borrower Rate + Charges
Customers whose Employment duration is high seem to lowest in delinquencing, also higher the available bank credit lower the delinquency
Higher the available bank credit lower is the Borrower APR
Higher the monthly payment, better is the Prosper score and vice versa
Full Time Employees have higher Prosper score with 8 being the median.
Unemployed customers have higher Borrower APR relatively around 0.33 as the median

Key findings of Analysis:

Unemployed customers who have chosen 36 months as the term for loan have the highest borrower APR It could be because of high risk involved in lending loan to unemployed since there was no fixed income at the time of applying loan
Maximum APR charged for the customers who have chosen 36,12months as term is same for all irrespective of employment statuses
Mean of Borrower APR is lower for home owners compared to Mean of Borrower APR of non home owners
Borrower APR and Prosper Score are negatively correlated

Resources:
Went through discussions in Stack Overflow forum while getting error for some commands.
