# customer_cancellation.
Introduction

The objective of this project was to understand the main reasons for customer cancellations in a company with over 800,000 clients. Through this analysis, I aimed to identify patterns and behaviors associated with churn and propose effective solutions to reduce this number.

Using data such as plan types, call center interactions, payment delays, and others, I conducted an in-depth analysis to pinpoint the most likely causes of cancellations. Additionally, I investigated ways to take proactive actions to improve customer retention and reduce churn, contributing to a more effective strategy for the company.
Dataset Overview

The dataset consists of 881,659 records and 11 columns, as described below:
Column	Description
idade	Customer's age.
sexo	Customer's gender.
tempo_como_cliente	Duration of customer relationship (in months).
frequencia_uso	Frequency of service usage (scale not defined).
ligacoes_callcenter	Number of calls made to the customer service center.
dias_atraso	Days overdue for payment.
assinatura	Type of subscription (e.g., Basic, Standard, Premium).
duracao_contrato	Duration of the contract (e.g., Monthly, Quarterly, Annual).
total_gasto	Total spending by the customer.
meses_ultima_interacao	Number of months since the last interaction.
cancelou	Whether the customer canceled (1 = Yes, 0 = No).
Data Cleaning

The dataset contained missing values, which were handled by removing any rows with null values. After cleaning, we maintained 881,659 records with no missing data.
Distribution of Cancellations

Initially, the distribution of cancellations was as follows:

    Cancelled (1.0): 499,993 customers (56.71% of the total).
    Not Cancelled (0.0): 381,666 customers (43.29% of the total).

After Data Filtering

To understand the reasons for customer cancellations, several filters were applied:

    Contract Duration: Removed customers with monthly contracts, as they were 100% likely to cancel.
    Call Center Interactions: Removed customers who contacted the call center more than 4 times, as they showed a tendency to cancel.
    Days Overdue: Removed customers who had more than 20 days of payment delay, as these customers always cancelled.

After applying the filters, the updated cancellation distribution was as follows:

    Cancelled (1.0): 85,447 customers (18.40% of the total).
    Not Cancelled (0.0): 379,032 customers (81.60% of the total).

Key Insights

After applying the filters, we observed the following key insights:

    Monthly plans: Customers with monthly plans were 100% likely to cancel. This suggests that the type of plan has a significant impact on customer retention.
    Call Center Interactions: Customers who contacted the call center more than 4 times tended to cancel. This indicates that frequent issues with the service may lead to dissatisfaction and churn.
    Payment Delays: Customers who were more than 20 days overdue on payments always cancelled, suggesting that payment delays are a major factor driving churn.

Conclusion

The filters applied allowed us to reduce the churn rate significantly, from 56.71% to 18.40%. This analysis shows that the following factors are strongly associated with customer cancellations:

    The type of contract, with monthly plans having a higher likelihood of churn.
    The number of interactions with the call center, indicating potential service dissatisfaction.
    Payment delays, with customers who are significantly overdue being more likely to cancel.

Based on these findings, we recommend that the company:

    Encourage customers to switch to longer-term plans (e.g., annual or quarterly).
    Improve the customer service experience to reduce the number of calls to the call center.
    Implement proactive measures for customers nearing payment delays to prevent cancellations.

By addressing these issues, the company can reduce churn and improve customer retention.
