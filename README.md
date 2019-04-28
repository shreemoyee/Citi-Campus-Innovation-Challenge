# Citi-Innovation-Campus-Challenge

## Problem Statement:
* Overpayment to a credit card account “could be used as a means to launder money because it provides
a simple means to convert criminal or suspicious funds [into] a bank instrument with minimal or no
questions as to the origin of the funds.”
* In this modus operandi, the cardholder makes a large payment (or multiple smaller payments in quick
succession) to his/her card account which exceeds the amount due, and via illicit (risky) means. They
then request the card-issuing institution to issue a rebate refund of this overpaid amount.
Risk Involved: The risk to the Firm of money laundering and/or terror financing.

## Objective:
You need to integrate the data given, club statements and payments, and use other relevant data to
develop features which would generate insights into the problem mentioned.
Please prepare a report of your approach, the report should explain the features created, their
relevance and credit cards ranking for suspicious cases based on below activities.

### Over payments:
* The more often a credit balance is over paid, the greater the risk
* The larger the amount exceeds the balance the greater the risk
### Refund:
* The more often a refund is requested, the greater the risk.

` Example `
A customer who has a debit(Purchases) of $3,000 in a statement period, makes a $4,000 credit
payment for the credit card bill.
So, The over payment = |Credit Payment – Debit Purchases| = $4,000 - $3000 = $1000.

## Data in scope:

• Payment for credit card bill.
• Purchase within statement periods.
• Rebate refund on transactions in statement periods.

The data is provided in the form of three csv and a xlsx:

### hackathon_payment_risk_data.csv 

 | Column | Description |
 | ------- | ------ |
| payment_channel_desc | Description of the type of payment say Cash payment |
| risk rating | The risk associated with the type of payment. 0 implies least risk while 10 implies highest risk |

### hackathon_all_data.csv 


| Column | Description |
| ---- | ---- |
| card number  | The credit card ID |
| Date | date |
| type_name | The type of data. This can be classified into purchases, payments, rebate refund and other categories  |
| payment_channel_desc | If the type_name as above is ‘PAYMENT’, this column gives the description of the type of payment |
| amountINR  | the amount associated (in Indian National Rupee)   |

### type_name_dictionary.xlsx 


| Column | Description |
| ----  | ------- |
| Type_name  | Transaction type categories say Payment  |
| Debit or Credit | The transaction is credit means it is incoming and debit is outgoing. |

### hackathon_statement_data.csv 

| Column | Description |
| ------- | --------- |
| card Number | the credit card ID  |
| billingStartDate  | the start of the billing period  |
| billingEndDate |  the end of the period   |
| paymentDueDate  | the date on which the payment is due for the purchases made between billingStartDate and billingEndDate  |

## Evaluation criteria:
You would be evaluated on your data understanding, EDA, Approach, Feature designing,
Visualization and Final Results.
