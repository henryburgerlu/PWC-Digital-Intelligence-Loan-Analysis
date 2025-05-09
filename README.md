# PWC-Digital-Intelligence-Loan-Analysis
This project was a part of the PWC Digital Intelligence job simluation program ob Forage: https://www.theforage.com/simulations/pwc-ch/digital-intelligence-kmu8

Objective: 
The goal of this project is to independently value a loan portfolio as of **31 December 2020**, in support of the client’s year-end audit based on the provided prompt and the dataset.

Dataset and informations:
The dataset includes **monthly loan origination amounts** and **observed repayments** for vintages between **June 2019 and December 2020**. We will compare our model outut with our clients to evluate absolute and relative difference. The client’s estimate of the portfolio value was CHF 84’993’122.67. We will compute both the absolute and relative difference. The audit team considers any difference smaller than CHF 500’000 to be acceptable given the size of the portfolio.

## The following assumptions are made to approach this project: 

Customers keep repaying at the same rate as before.

There’s no increase in defaults or economic shocks.

No write-offs or losses are anticipated.

A 5% annual discount rate is used, converted to a monthly rate for DCF purposes.

The discount rate remains constant across the entire forecast period and does not reflect changing market or credit risk conditions.

## Approach to the project: 

First, we look at histoical actual repayment percentages for each vintage across observed months by dividing repayments across all vintages.

Second, Using the histoical average of repayment across all vintage, we find the 20-month expected repayment curve. 

Cash Flow Forecasting: Applying the expected repayment percentage to each vintage's original amount to project future monthly cash flow January 2021 onward. 

Applied Discounted Cash Flow Value: Say we used a 55 annual discount rate and convert it to monthly to discount the forecasted absolute and relative differences. 

Variance Analysis: Compare our model's evaluation with our client's provided estimation of CHF 84,993,122.67

Assessment Outcome for recommendations: Evaluated whether the difference exceeded the audit materiality threshold of CHF 500,000.

# Conclusion
Based on the expected repayment percentages provided and a 5% annual discount rate, our model estimates the portfolio value as of 31 December 2020 to be CHF 137,876,240.63, which exceeds the client’s estimate of CHF 84,993,122.67 by approximately CHF 52.88 million (+62.22%).

The model suggests significantly higher value than the client’s estimate.

Forecasted repayments appear optimistic based on historical averages.

The client may be:

Using a more conservative repayment assumption

Accounting for defaults, charge-offs, or economic risk not modeled here

Our model assumes full repayment according to historical averages, whereas the client may have factored in expected credit losses, delinquency, or write-offs.

It is suggested that it might be helpful to reconcil assumptions with the client — particularly around repayment expectations, loss assumptions, and discounting methodology — to ensure alignment for audit validation and financial reporting.

