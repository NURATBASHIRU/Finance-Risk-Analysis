## Finance-Loan-Analysis

#### Title: Finance Loan Analysis – Risk and Loan Default Analysis.
![Screenshot 2024-09-30 094841](https://github.com/user-attachments/assets/1d0fe54b-9959-4701-9f02-75352bf3a0d8/image.png)

Objective: This project is a Risk and Loan Default Analysis performed for a financial institution to better understand it operations, loan default and turn-over rate. This analysis will help this finance company develop strategies that would improve it turn-over rate, profit and its entire operations.
This Analysis answers the following questions; 
- What is the loan default rate by customer demographics (e.g., income, employment length)?
- Identify the interest rates and their impact on loan performance. 
- What are the loan amounts across different customer segments and loan purposes?
- What is the loan approval rates by region and customer risk profiles.
Methodology;
-	Tool: Microsoft Excel
-	Technique: Using the member’s LTV (Loan To Value) Ratio and DTI (Debt To Income) Ratio, I was able to group these customers based on similar earning / debt category.
-	Process: I performed an intensive data cleaning procedure on the dataset and the procedure required me to create a few new columns. As a result, the dataset increased from 26 columns and 38,590 rows to 30 columns and 38,575 rows.
Transformation Process
Transforming this dataset would have been a little more difficult if a “data dictionary” was not created by TDI. However, the following are the data transformation process the dataset went through;
1.	I performed an overall data cleaning procedure using; trim, proper and text functions
2.	Blanks: I used the Find and Replaced feature of Excel to replace empty cells in “job role” column with “others” – so that all members can be evenly categorized. I also did the same with the “total payment” column. I replaced empty cells in “total payment” column with 0.
3.	Data Normalization: I used VLOOKUP function to convert the “Address State” column from Alpha 2 area code to actual state name. I used the IF statement to group the interest rate into 3 categories – “low interest rate”, “mid interest rate” and “high interest rate”. I converted “Home Ownership” column from abbreviation to words; Home ownership status of members was in “R, MO, O, NONE format” (R-RENT, MO- MORTGAGE, O-OWN). I applied the same process for the “Verification Status” column as it was in; V-Verified, NOT V- Not Verified, SV- Source Verified format.
4.	Incomplete Metrics: I created a new column – LTV - derived LTV (Loan to Value) by using “Annual income” as collateral. So, LTV = Loam amount/Annual Income X 100. I created a “loan Deficit” Column by using; loan amount - Total payment.
5.	Duplicates: Removed 15 duplicates and as a result, the dataset when from 38,590 records to 38,575 unique records.

![Screenshot 2024-09-30 0952391](https://github.com/user-attachments/assets/89f3ff8d-0093-4271-ba2e-db05d1c76c05)

Insights
1.	The finance company has a total loan approval of $473 million with a $435.7 million retrieved and a default of -$37.3 million - losing about 10% of its principal. 
2.	Members who have long term work experience have the highest default rate
3.	High interest rate is deeply associated with the default rate.
4.	Members who own houses on mortgage have the highest loan approval rate followed by members who live in rented houses. While members who own their homes get a really low percentage of loan approval, members who do not own a house barely get loan approval - for obvious reasons.
5.	California, New York and Texas are the highest loan approval rate and consequently, the highest default rate.

Recommendation 
1.	The finance company should review it loan policy generally to reduce loan defaults. High interest rate is associated with high default rate. So, the company should review its interest rate to make it easy for borrowers to pay-up.
2.	Proper assessment of collateral value and debt to income ratio would lead to realistic credit scores and reduce default rate in the long-run.
3.	The company should increase it loan approval rate for home owners - as long as the borrower’s property meets the collateral policy.
