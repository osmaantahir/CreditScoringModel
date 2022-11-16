# CreditScoringModel

Purpose of this model is to parse transactional data of 6 months and assign credit limits as retailers buying behavior.

## Whitelisting
All retailers are filtered as per minimum criteria of atleast 10 transactions and 30 days recency so that retailer profile can developed. At this stage blacklisting and delinquences are also checked from credit bureau due to confidentiality reasons and do not want to disclose database schema it is omitted and inputed as excel file after running sql queries from transactional and credit bureau db.

## Segmentation
All retailers are then fed into RFM Analysis and then classified into four segments through quantiles.

## Demand Forecasting
SARIMAX is used for demand forecasting.

## Credit Limit Assignment
Risk appetite rule is defined and map to each segment of the retailer for credit limit assignment.
