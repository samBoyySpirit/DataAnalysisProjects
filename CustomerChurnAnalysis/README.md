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