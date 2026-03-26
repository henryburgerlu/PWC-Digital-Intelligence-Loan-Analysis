# PWC-Digital-Intelligence-Loan-Analysis
This project was a part of the PWC Digital Intelligence job simulation program from Forage: https://www.theforage.com/simulations/pwc-ch/digital-intelligence-kmu8

Objective: 
The goal of this project is to independently value a loan portfolio as of 31 December 2020, in support of the client’s year-end audit based on the provided prompt and the dataset.

Dataset and informations:
The dataset includes monthly loan origination amounts and observed repayments for vintages between June 2019 and December 2020. We will compare our model output with our clients to evaluate absolute and relative difference. The client’s estimate of the portfolio value was CHF 84’993’122.67. We will compute both the absolute and relative difference. The audit team considers any difference smaller than CHF 500’000 to be acceptable given the size of the portfolio.

## The following assumptions are made to approach this project: 

Customers keep repaying at the same rate as before.

There’s no increase in defaults or economic shocks.

No write-offs or losses are anticipated.

A 5% annual discount rate is used, converted to a monthly rate for DCF purposes.

The discount rate remains constant across the entire forecast period and does not reflect changing market or credit risk conditions.

## Approach to the project: 

First, we look at historical actual repayment percentages for each vintage across observed months by dividing repayments across all vintages.

Second, Using the historical average of repayment across all vintage, we find the 20-month expected repayment curve.

Cash Flow Forecasting: Applying the expected repayment percentage to each vintage's original amount to project future monthly cash flow January 2021 onward.

Applied Discounted Cash Flow Value: Say we used a 55 annual discount rate and convert it to monthly to discount the forecasted absolute and relative differences.

Variance Analysis: Compare our model's evaluation with our client's provided estimation of CHF 84,993,122.67

Assessment Outcome for recommendations: Evaluated whether the difference exceeded the audit materiality threshold of CHF 500,000.

# Conclusion
Based on a month-in-life aligned repayment curve and a 5% annual discount rate, our model independently estimates the portfolio value as of 31 December 2020 to be CHF 102,291,840.95.

This is higher than the client's estimate of CHF 84,993,122.67, resulting in an absolute difference of CHF 17,298,718.28 (+20.35% relative to the client's estimate). Since this difference exceeds the CHF 500,000 audit materiality threshold, it indicates a notable discrepancy in the valuation that warrants further investigation.

Forecasted repayments are based strictly on observed historical averages across all loan vintages, weighted by origination amount and aligned by month-in-life position.

The model operates under the following assumptions:

Customers continue to repay at historical average rates
No increase in defaults or economic shocks
No write-offs or losses are anticipated
A constant 5% annual discount rate applies throughout the forecast period
The remaining gap of CHF 17.30 million suggests the client's estimate may incorporate one or more of the following adjustments not reflected in our model:

Expected credit losses or anticipated loan defaults
A more conservative or alternative repayment curve
A different discount rate or discounting horizon
Provisions for charge-offs, delinquency, or economic risk
The model assumes full repayment in line with historical averages, whereas the client may have applied credit loss expectations or other risk adjustments.

It is recommended to reconcile assumptions with the client — particularly around repayment expectations, loss provisioning, and discounting methodology — to ensure alignment for audit validation and financial reporting purposes.
