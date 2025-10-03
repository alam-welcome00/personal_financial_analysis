# Personal Financial Overview Dashboard
### 📌 Project Overview

This project is a self-driven data analytics case study where I analyzed my own banking transactions to gain insights into my personal financial habits. Using Excel for data cleaning and Power BI for visualization, I built an interactive dashboard to track income, expenses, savings, and spending trends.

### 📂 Data Source & Preparation

Exported statements from two different banks (PDF format).

Converted statements into Excel for preprocessing.

Cleaning steps included:

Removing redundant columns and text noise from PDF exports

Using formulas like IF, SUBSTITUTE, TRIM to fix messy entries

Standardizing date, amount, and transaction type fields

Creating a Month-Year column for time-based analysis

Classifying transactions as Credit (inflow) or Debit (outflow)

### 📊 Analysis Performed

The cleaned dataset was analyzed to answer key financial questions:

Average Monthly Income & Expense → Am I living within my means?

Debit vs Credit Counts → How many inflows vs outflows?

Monthly Expense Trends → Which months had higher spending and why?

Transaction Segmentation → Grouping by categories (Bills, Shopping, Rent, Salary, etc.)

Max/Min Analysis → Highest single expense, lowest expense month, and savings %

### 🧮 Major DAX Functions Used

Some important DAX calculations that powered the dashboard:

- Total Income

        Total Income = CALCULATE(SUM(Transaction[Amount]), Transaction[Type] = "Credit")

- Total Expense

        Total Expense = CALCULATE(SUM(Transaction[Amount]), Transaction[Type] = "Debit")

- Net Savings

        Net Savings = [Total Income] - [Total Expense]

- Average Monthly Expense

        Avg Monthly Expense = AVERAGEX(VALUES(Transaction[Month-Year]), [Total Expense])

These measures allowed me to dynamically calculate KPIs and visualize spending vs saving patterns across time.

### 🎨 Dashboard Design (Power BI)

Key features of the dashboard include:

Dark-themed design with transparent visuals

KPI Cards for Total Income, Expense, and Savings

Line Chart showing monthly net transactions

Bar Chart highlighting monthly expense trends

Donut Chart for category-wise spending

Cards showing highest and lowest expense months

### 💡 Why This Project Matters

This was not based on sample datasets — I worked with real-world messy banking data.

It gave me practical experience in data cleaning, shaping, and visualization.

Helped me discover personal finance insights and improve my Excel + Power BI + DAX skills.

Proved the value of DIY analytics in turning raw financial statements into actionable insights.

### 🛠️ Tech Stack

- Excel → Data Cleaning & Preparation

- Power BI → Data Modeling, DAX, Visualization

## Dashboard
<img width="1920" height="1200" alt="Image" src="https://github.com/user-attachments/assets/194a9b37-c780-4222-be9f-0855310afe02" />
