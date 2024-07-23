# Lending Club Case Study
> This project aims to identify patterns that indicate if a person is likely to default on a loan. These insights can help take actions such as denying the loan, reducing the loan amount, or lending at a higher interest rate. The goal is to reduce credit loss using exploratory data analysis (EDA).


## Table of Contents
* [General Info](#general-information)
* [Tools and Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Contact](#contact)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Project Overview: A consumer finance company, Lending Club, specializes in offering various types of loans to urban customers.

- Background: When a loan application is received, the Lending Club must decide whether to approve the loan based on the applicant’s profile. The company faces two types of risks:
If the applicant is likely to repay the loan, not approving it results in a loss of business.
If the applicant is likely to default, approving the loan may lead to a financial loss.

- Business Problem: The Lending Club platform needs insights to assess the loan approval/rejection risk. This study uses loan history data from 2007 to 2011 to identify the driving factors for loan defaults.

- Dataset: Loan history data from 2007 to 2011.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Tools and Technologies Used
To run this project, you need to have Anaconda Jupyter Notebook and Python installed along with the following libraries:
- pandas
- numpy
- matplotlib
- seaborn
- warnings

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Conclusions
### Univariate Analysis Observations:
- Loan Amounts: More defaulters are observed with loan amounts between $3,000 and $12,000.
- Annual Income: Many defaulters have annual incomes between $2,000 and $8,000.
- DTI Value: The number of defaulters increases with higher DTI values.
- Interest Rates: Defaulters are more common with interest rates between 10% and 18%.
- Loan Status: The distribution of loan status is consistent across loan amounts.
- Interest Rate for Defaulters: Defaulters have higher interest rates compared to fully paid loans.
- Homeownership: Defaulters are ranked as RENT > MORTGAGE > OWN > OTHER.
- Verification Status: Defaulters are ranked as Not Verified > Verified > Source Verified.
- Purpose: Debt consolidation is the most common purpose among defaulters.
- Employment Length: Defaulters with 10+ years of employment are notably high.
- Grade: Defaulters are ranked as B > C > D > A > E > F > G.
- Term: Defaulters with a 36-month term are more common than those with a 60-month term.
- Address State: California (CA) has the highest number of defaulters, followed by Florida (FL), New York (NY), Texas (TX), and New Jersey (NJ).
- Monthly Trends: The number of defaulters is increasing monthly.
- Yearly Trends: The number of defaulters is increasing yearly.

### Observations from Bivariate Analysis:
- Grades: Defaulters are predominantly in grades B and C. Subgrades B3, B4, B5, C1, C2, and C3 have the highest number of defaulters.
- Verification Status: Across all homeownership types, the "Not Verified" status is most common among defaulters. For RENT homeownership, defaulters are equally distributed between "Source Verified" and "Verified" statuses.
- Purpose: Debt consolidation is the most common purpose among defaulters across all homeownership types. For RENT homeownership, the second most common purpose is "other," while "home improvement" ranks second and "credit card" third for MORTGAGE homeownership.
- Employment Length: Defaulters with 10+ years of employment are most common across all homeownership types. For RENT homeownership, the second highest category is "< 1 year" and the third is "2 years," whereas for MORTGAGE homeownership, "3 years" ranks second and "5 years" third.
- Grades and Verification Status: For grades A to D, the "Not Verified" status is more common, while for grades E to G, the "Verified" status is more prevalent.
- Grades and Purpose: Across all grades, debt consolidation is the most common purpose. For grades A to D, the second most common purpose is "other," whereas for grades E to G, "small business" takes the second spot.
- Grades and Employment Length: Defaulters with 10+ years of employment are more common across all grades.
- Grades and Homeownership: Defaulters are more commonly associated with RENT and MORTGAGE homeownership.
- Verification Status by Employment Length: Across all employment lengths, the "Not Verified" status is more prevalent. However, for employees with 10+ years of experience, the "Verified" status is more common.
- Employment Length and Grades: Employment lengths of 1 year, 10+ years, 2 years, 4 years, 5 years, 7 years, and 8 years have more Grade B defaulters, while 3 years, 6 years, 9 years, and less than 1 year have more Grade C defaulters.
- State Observations: Verification status "Not Verified," employee lengths of 10+ years and less than 1 year, and homeownership "RENT" are prevalent across many states. Particularly in California (CA), RENT homeownership is the most common among defaulters.
- Interest Rates and Defaulters: As interest rates increase, the number of defaulters rises, regardless of annual income and loan amount. Defaulters are more common with interest rates of 12.5% or higher.
- Annual Income and Defaulters: Applicants with lower annual incomes are more likely to default compared to those with higher annual incomes.

### Observations from Multivariate Analysis:
- Loan Amount and Grade: The negative correlation between loan amount and grade indicates that lower loan amounts are associated with better grades among defaulters.
- Loan Amount and Annual Income: A correlation of 0.37 between loan amount and annual income shows a moderate positive relationship. This suggests that as annual income increases, the loan amount tends to increase as well, although the correlation is not very strong.
- Grade and Interest Rate: The strong positive correlation between grade and interest rate indicates that higher loan grades are associated with lower interest rates among defaulters.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Contact
Created by [https://github.com/udaykiranpujaari72] [Vaibhav Agarwal] - feel free to contact us!
