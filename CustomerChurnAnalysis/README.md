# Scenario.

CageTel (Cage Telecommunications Inc.) is a fictitious telecom company owned by Nicolas Cage(not really), that provides home phones and Internet services to 7043 customers in California Q3.

CageTel is facing a **Customer Churn** issue recently. Nicolas Cage has ordered the Company to retain it's customers by analyzing all relevant Customer data and determine their behaviour patterns. Nic Cage wants CageTel to develop focused customer retention programs.

## What is Churn analysis?
Churn analysis is the evaluation of a company's customer loss rate in order to reduce it. Also referred to as customer attrition rate, churn can be minimized by assessing your product and how people use it.

# Stage 1: Ask.

## Requirement:

To determine the behaviour of customers and to develop focused customer retention programs. In short, minimize the Customer Churn.

## Stakeholders:
* Nicolas Cage, Director of CageTel, who is the primary stakeholder for this project.
* Marketing Team, they are secondary stakeholders.
* Data & Analytics Team, that has to create a dynamic dashboard and provide insights from the data gathered.

## Business Task:

Create a detailed analysis of the customer data so as to identify the reason for customer churn and develop a dashboard to provide quick insights.

## Expectation: 

Top 3 recommendations on how to reduce Customer Churn for CageTel.

## Stack:
* Data source: .csv file. Dataset can be downloaded here: <https://www.kaggle.com/datasets/blastchar/telco-customer-churn>.
* Data processing: Python Pandas Library.
* Data Visualization: Python Pandas, Seaborn Library.

# Stage 2: Prepare.

## About the data:
Each row represents a customer, each column contains customer’s attributes.
The data set includes information about:
* Customers who left within the last month – the column is called Churn.
* Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies.
* Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges.
* Demographic info about customers – gender, age range, and if they have partners and dependents.

Download the dataset from here <https://www.kaggle.com/datasets/blastchar/telco-customer-churn>.

# Stage 3: Process.

EDA, data cleaning and the feature analysis will be performed and documented in `cagetel_customer_churn_analysis.ipynb`.

# Stage 4: Analysis.

## Research questions to consider.

* Explore the dataset and find the relationships between People Demographics, Customer Account Details and Services provided.
* What is the customer churn rate?
* How does Gender and Senior Citizen affect Churn rate?
* Does customers having dependents affect customer Churn?
* How does customer churn relate with tenure?
* Which contract type has higher churn rate?
* How does the various service provided by the telco company affect churn?
* Determine what kind of services were used by unsubcribed(churned) customers.
* Does having no tech support influence customer churn?
* How are the Monthly and Total charges contributing to customer churn?

# Stage 5: Share.

## Key Insights:

* About 27% of the customers have churned in this dataset.
* Gender has very less influence on Churn rate in this dataset.
    - The distribution of male female gender is almost 50-50%
    - Around 26% male and 27% female in this dataset have churned.

* The dataset contains of 83.8% non-senior citizens customers and the rest 16.2% are senior citizens.
    - Amongst the churned customers, 74.5% of them are non-senior citizens.
    - This means that the CageTel is losing younger customers and the older ones have been largely loyal.
    - Out of 1393 non-senior citizens that have churned, 1214 of them had month-to-month contract type.

* About 70% of the customers in this dataset have no dependents.
    - 82.5% of the customers who have churned have no dependents.
    - Having no dependents is one of the factors that make it easy for customer's to leave/unsubscribe.
    - Even amongst the customers who have remained with the company, about 65.66% have no dependents, while the remaining do.

* Tenure(months) has a negative correlation with churn, i.e., customers who have churned have been with the company for lesser tenure.
    - Customers who have churned, their average tenure is 10 months or less. In this short period, the company hasn't provided value to these customers for them to stay.
    - Long time customers have stayed with the company for an average of 40 months.
    - For the customers that have not churned, two-year contract types have the highest tenure(60-70 + months).
    - Month-to-month contract types have mostly customers churning with tenure around 1-3 months.

* Out of 1869 customers that have churned, 69% of them had Fiber Optic Internet service. This could mean that the Fiber Optic service provided by the company has not provided value to these customers.
    - The average tenure of churned customers who had opted Fiber Optic internet service is 12 months.
    - The Fiber optic Internet service is one of the factors that is positively correlated to churn.

* Payment Method option *Electronic Check* is one of the factors that have positive correlation with Churn.
    - 57.3% of the churned customers had Electronic Check payment type. This could possibly mean that this type of payment method has issues which is leading unsatisfied customers.

* In general, large number of customers in this dataset have no customer support. This could be improved and customer tech support could be utilized to build customer retaining programs.
    - Among the churned customers, 83.4% of them had no tech support part of their product offering.
    - Customers who have stayed with the company for longer tenure have opted for Tech support. This could mean that either long term contracts(one or two-year one's) have been bundled with tech support and it has provided value add.
    - Maybe introducing tech support to the month-to-month contract type could help retain customers.

*  Customers with higher monthly charges are more likely to churn.
    - Lesser overall total charges is seen to have less churn rate.

# Stage 6: Act

## Top 3 recommendations.

* To retain younger and non-senior citizens, add value add features to product offerings.
    - Add tech support to the month-to-month contracts and any other small value add feature.
    - Enable month-to-month contract customers to upgrade to longer contracts(one or two-year contracts) by giving discounts.
* Make it easy for customers to add dependents to plans or contracts. Adding dependents will reduce the likeliness of churning.
* Fix issues relating to the Fiber Optic Internet service as this is one of the major factors contributing to churn.

**Bonus Tip:** Make a marketing ad with the *`Greatest Living Actor in all Universe`*, Nicolas Cage, to show just how cool CageTel is.
![Deal with it!!](images/deal-with-it-nic.gif)

# Acknowledgement.

I have used the following sources as references to learn and build my own analysis of the customer churn dataset.
* <https://www.kaggle.com/code/bandiatindra/telecom-churn-prediction/notebook>
* <https://jovian.ai/rrahul1011/data-analysis-project-telco-customer-churn>
* <https://github.com/YuehHanChen/Telco_Customer_Churn_Analysis>

Thanks to the respective authors.