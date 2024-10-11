# Quaint Finance Modeling
## Background Information
Today, credit is no longer limited to classical bank loans. The rise of e-commerce has increased the demand for new and more flexible credit solutions. The increased demand has been met by new companies from the fintech sector that offer easily accessible online loans to a wide audience. These new business models offer simple solutions, such as flexible payment schedules or buy-now-pay-later, that can be accessed with just a few clicks. 

Online merchants also need new ways to procure capital to manufacture their products, as they receive payment only after their product has been sold. In order to meet increasing demand, new credit offerings have emerged. Repayment of these loans is no longer based on a fixed schedule but instead depends directly on online sales. The loan is paid back in instalments with every sale, and thus payments depend directly on the sales volume. 

## Project Overview
we will walk through the valuation process of a merchant loan portfolio for a global online lending platform.
This evaluation is critical as it directly impacts the balance sheet, and we need to ensure accuracy for the year-end audit as of December 2020.

## Business Understanding
The client offers loans to merchants, which are classified as assets.
These loans are repaid based on the merchants' sales, not a fixed schedule.
This unique repayment structure requires us to forecast future cash flows in order to value the portfolio accurately.
Our goal is to compare our valuation against the client’s and check if it falls within an acceptable threshold.

## Data Understanding
The historical data includes loans originated each month (vintages) from June 2019 to December 2020, along with observed repayments.
For each month (vintage), we have the loan amounts and repayments.
We will use this information to compute the repayment percentages and forecast future repayments over the loan's lifetime.

## Loan Valuation
First, we calculate historical repayment percentages, which is simply the ratio of repayments to the amounts originated per vintage.
Next, we compute expected repayment percentages for future periods based on the observed trends from the historical data.
Finally, we forecast the future cash flows by applying these expected percentages to the amounts originated for each vintage.

To compute the present value (PV) of the forecasted cash flows, we use a discount rate of 2.5%.
This annual rate is converted to a monthly rate, and then we apply it to discount future cash flows back to their value in December 2020.
The PV calculation gives us the current value of the expected future repayments.

##  Results Comparison
The client’s original valuation of the portfolio was CHF 84,993,122.67.
We will present our calculated portfolio value and the absolute and relative differences between our estimate and the client's.
Based on our analysis, we will determine whether the portfolio value is within this acceptable range or not

## Findings
The fair value estimate for the portfolio is 42792456.39 Swiss Francs.
After analyzing the data and performing the valuation, we concluded that the calculated portfolio value is within the acceptable range set by the audit team which was below CHF 500,000.
This validates the client's balance sheet valuation and ensures accuracy for the year-end audit.
