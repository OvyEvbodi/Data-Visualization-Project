# Prosper Loan Exploration
## by Ovy Evbodi


## Dataset


This is a loan dataset from ProsperLoans that contains various variables related to their borrowers and the company's loan services. The dataset was provied by [Udacity](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv) and this helpful [data dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0) sheds some light on the various variables.
Some columns were names didn't follow the python conventional naming protocol. I renamed those columns(ListingCategory (numeric)': 'ListingCategory', 'ProsperRating (numeric)', 'ProsperRating (Alpha)', 'TradesNeverDelinquent (percentage)') before being able to plot visualizations on them. I changed the datatype of the "DataCreditPulled" column in order to be able to reference the values as a Datetime format for accurate analysis.
I created two new columns from the existing listing category and loan status variables because I wanted to narrow down my analysis. For the loan status, the new column contains only values where the loan status is either 'completed' or 'defaulted', while for the listing category, I focused on just 'debt consolidation', 'home improvement', and 'business'.


## Summary of Findings


From my analysis, I was able to visualize how factors like APR, loan amount, listing category and some other factors influence the outcome of a loan status. The borrower APR of a loan has a relationship with the loan status of that loan in that the higher the APR, the higher the probabilty of the borrower defaulting in the payment of that loan.

The employment status doesn't seem to have any relationship with a borrower defaulting in loan payment. Over 80% of borrowers in each category completed their loan payment when compared to those who defaulted in their payment.
 
While debt consolidation was the number one reason people took out loans(regardless of their employment status), a higher proportion of self-employed people took out more business loans compared to people from other categories of employment. 'Student use' was the second most common reason borrowers with part-time employment took out loans.

Debt consolidation loans with a higher APR had more defaulters.

The number of recommendations a borrower has also seems to have a positive correlation with the loan status, borrowers with more recommendations tend to payoff their loans more than those with fewer recommendations.

Generally, the loans that get cancelled do not exceed \$5000.

## Key Insights for Presentation
 
 
My key insights presented were visualizations on the effect of the employment status on the loan status outcome, the relationship between the listing category, apr and loan status, and how recommendations and the loan amount of a loan affect the loan status outcome of that loan.




