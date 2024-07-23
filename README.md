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

### Key Insights from Analysis:
- **Loan Amount and Default Risk**:
  - **Insight**: Loans between $3,000 and $12,000 are at a higher risk of default.
  - **Analysis**: Smaller loan amounts often correlate with higher risk grades, suggesting increased vigilance for these loans.

- **Annual Income and Default Risk**:
  - **Insight**: Default risk is notably higher for applicants with annual incomes between $2,000 and $8,000.
  - **Analysis**: Lower income levels are a significant predictor of default, while higher incomes are generally associated with larger, less risky loans.

- **Debt-to-Income (DTI) Ratio**:
  - **Insight**: An elevated DTI ratio is a strong indicator of potential default.
  - **Analysis**: Applicants with higher DTI ratios struggle more with debt management, heightening the risk of default.

- **Interest Rates**:
  - **Insight**: Higher interest rates (10%-18%) are linked with increased default rates.
  - **Analysis**: Elevated interest rates are often associated with higher-risk loans, requiring careful assessment.

- **Homeownership and Default Risk**:
  - **Insight**: Renters have the highest default rates, followed by mortgage holders, with homeowners being the least likely to default.
  - **Analysis**: Homeownership status is a critical factor in determining default risk, with renters posing the greatest risk.

- **Verification Status**:
  - **Insight**: Applicants who are "Not Verified" show a higher likelihood of default.
  - **Analysis**: Ensuring thorough verification can significantly reduce the risk of default.

- **Purpose of Loan**:
  - **Insight**: Loans for debt consolidation have the highest default rates.
  - **Analysis**: These loans should undergo stringent scrutiny to mitigate associated risks.

- **Employment Length and Default Risk**:
  - **Insight**: Default rates are notable among applicants with over 10 years of employment and those with very short employment durations.
  - **Analysis**: Employment length should be considered in conjunction with other risk factors for a comprehensive assessment.

- **Loan Grades**:
  - **Insight**: Grades B and C, particularly subgrades B3, B4, B5, C1, C2, and C3, have the highest default rates.
  - **Analysis**: Loans in these grades need more rigorous evaluation due to their higher default risk.

- **Loan Term and Default Risk**:
  - **Insight**: Loans with a 36-month term have a higher default rate compared to those with a 60-month term.
  - **Analysis**: The increased monthly payment burden of shorter-term loans contributes to higher default risk.

- **Geographic Location**:
  - **Insight**: States such as California, Florida, New York, Texas, and New Jersey have the highest default rates.
  - **Analysis**: Regional economic conditions and living costs are significant factors influencing default rates.

- **Trends Over Time**:
  - **Insight**: Default rates have been rising steadily both on a monthly and yearly basis.
  - **Analysis**: Continuous refinement of risk assessment strategies is essential to adapt to these trends.

- **Loan Amount and Grade**:
  - **Insight**: There is a negative correlation between loan amount and grade.
  - **Analysis**: Lower loan amounts are associated with better grades among defaulters, indicating that smaller loans are generally tied to better credit scores.

- **Loan Amount and Annual Income**:
  - **Insight**: A correlation of 0.37 between loan amount and annual income suggests a moderate positive relationship.
  - **Analysis**: As annual income increases, the loan amount tends to rise as well, although the correlation is not very strong.

- **Grade and Interest Rate**:
  - **Insight**: A strong positive correlation between grade and interest rate.
  - **Analysis**: Higher loan grades are associated with lower interest rates among defaulters, implying that better grades generally receive lower interest rates.


### Recommendations

1. **Strengthen Verification Processes**
   - **Action**: Enhance verification procedures for loan applicants.
   - **Rationale**: By reducing the number of "Not Verified" applicants, default risks can be significantly mitigated.


2. **Focused Risk Assessment**
   - **Action**: Pay special attention to mid-range loan amounts, lower annual incomes, higher DTI ratios, and elevated interest rates.
   - **Rationale**: These factors are critical indicators of increased default risk and warrant closer scrutiny.


3. **Develop Geographic and Purpose-Based Policies**
   - **Action**: Implement targeted policies for high-risk geographic regions and specific loan purposes, especially debt consolidation.
   - **Rationale**: Tailored policies address the unique risks associated with different geographic areas and loan purposes.


4. **Comprehensive Risk Evaluation**
   - **Action**: Integrate various risk factors, such as employment length, loan grade, and term duration, into the evaluation process.
   - **Rationale**: A holistic evaluation approach provides a more accurate assessment of default risk.


5. **Ongoing Monitoring and Adaptation**
   - **Action**: Regularly review and update risk assessment strategies to align with current trends and emerging data.
   - **Rationale**: Proactive and adaptive strategies will enhance the effectiveness of risk management practices.


## Contact
Created by [https://github.com/udaykiranpujaari72] [Vaibhav Agarwal] - feel free to contact us!
