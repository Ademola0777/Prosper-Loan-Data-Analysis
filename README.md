# Prosper-Loan-Data-Analysis
 The dataset used for this project is the Prosper Loan Dataset. The dataset contains data about the details of the various loans lent to the borrowers from Prosper. Each row in the dataset represents a loan, uniquely identified by the Listing Key.
Every row in the dataset describes various attributes about the Borrower such as Employment Status, Credit Score, etc. Every row also describes other parameters such as Monthly Payments, On Time Payments, Interest Rate, etc.
Dataset
The Prosper loan dataset comprises of 113937 loan entries with 81 attributes on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others, from the year 2009-2014. There are two main categories:
# Key Intrest
Borrower information: Basic attributes of the borrowers such as annual income, condition of employment, interest rate, loan status, etc.
Loan performance information: Metrics evaluating the risk associated with the loans such as Prosper score and bank card utilization, etc. There were some elements that need to be fixed, in order to create interesting and trustworthy analyses and visualizations.
Summary of Findings
The objective of this work is to investigate factors affecting borrower rate and loan amount:
# What features in the dataset do you think will help support your investigation into your feature(s) of interest?
Supporting features in the dataset includes borrower details (e.g., ProsperRating, IncomeRange, DebtToIncomeRatio) and loan attributes (e.g., LoanOriginalAmount, LoanTerm, ListingCategory).

Loan performance metrics like LoanStatus, PastDueAmount, and OnTimeProsperPayments track repayment behavior. This data supports analyzing borrower profiles, loan trends, and risk-return patterns.

# The Prosper dataset shows:

Loan Amount: Positively skewed with outliers; log transformation applied.
Emplyment Status: Uniform mid-range distribution; no transformations needed.
Income Range: Dominated by mid-range incomes; low-frequency categories grouped.
Loan Term: Multimodal (12, 36, 60 months); no transformations required.
Loan Purposes: Most borrowers get loan for debt consolidation
Key patterns and necessary adjustments were identified for analysis.

I reduced the number of income ranges by one by merging USD 0 with Not Employed into the same category.
I further looked at a couple of right skewed variables using a logarithmic scale to better see where the bulk of the data points lie.
Most of my cleaning efforts and adjustment were on ordering factors levels to make more intuitive sense

# Relationship observed during analysis
Income and Employment strongly influence loan amounts and approval likelihood, with employed borrowers and those in specific income ranges being more likely to take out larger loans.
Debt-to-income ratio plays a crucial role in the size of the loan a borrower receives, with lower ratios correlating with higher loan amounts.
Loan terms tend to be set at 36 months, indicating that borrowers prefer manageable repayments.
Debt consolidation is the most common loan purpose, suggesting many borrowers are using loans to restructure or pay off existing debts.
These relationships underscore how various factors such as income, employment, debt-to-income ratio, and loan purpose influence borrowing behavior and the lending process on Prosper.

# Conclusions
The Prosper dataset reveals key insights into loan origination patterns and borrower behavior. The loan amount distribution is trimodal, with common loan amounts at 5,000, 10,000, and 15,000, suggesting borrowers often seek loans in these ranges. Borrowers with higher stated monthly incomes tend to have loan spikes around specific income values like 4,000, 4,500, and 5,000 after outliers are filtered. Employed individuals are more likely to take out loans, and the majority prefer a 36-month loan term. Over 60% of borrowers are homeowners, indicating a relationship between homeownership and loan acquisition.

A significant proportion of loans are issued to borrowers with a low debt-to-income ratio, particularly for larger loan amounts. Most loans are used for debt consolidation, reflecting a common trend of borrowers using loans to pay off existing debt. Additionally, the year 2013 stands out as the peak year for loan originations, and current loans dominate the dataset, suggesting many loans remain active.

In summary, Prosper’s dataset highlights trends in borrower behavior, loan preferences, and financial health, offering insights into how borrowers use loans primarily for debt management and how loan terms, income, and employment status influence lending patterns.
