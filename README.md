Retail Sales Analytics Dashboard
Overview

The Retail Sales Analytics Dashboard is an end-to-end data analytics project that transforms raw retail sales data into actionable business insights. Using Python, SQL, and Power BI, the project analyzes sales performance, customer behavior, product profitability, and regional trends to support data-driven decision-making.

Problem Statement

Retail businesses generate large volumes of transactional data daily. Without proper analysis, valuable insights regarding sales growth, customer preferences, and product performance remain hidden.

This project addresses that challenge by creating a centralized analytics dashboard that enables stakeholders to monitor key business metrics and identify growth opportunities.

Objectives
Analyze sales and profit performance.
Identify top-performing products and categories.
Understand customer purchasing behavior.
Evaluate regional sales trends.
Build an interactive dashboard for business reporting.
Tech Stack
Category	Tools
Programming	Python
Data Analysis	Pandas, NumPy
Database	SQL
Visualization	Matplotlib, Seaborn
Dashboard	Power BI / Tableau
Development	Jupyter Notebook
Dataset

The dataset contains retail transaction records including:

Order ID
Order Date
Customer Information
Product Details
Sales Amount
Profit
Quantity
Region
Category

Project Workflow
1️⃣ Data Collection
Import retail sales dataset.
Validate data quality and completeness.

2️⃣ Data Cleaning
Handle missing values.
Remove duplicates.
Standardize column formats.
Convert data types.

3️⃣ Exploratory Data Analysis (EDA)
Sales trend analysis.
Profitability analysis.
Category-wise performance.
Customer behavior analysis.

4️⃣ SQL Analysis
Revenue calculations.
Top product identification.
Customer insights.
Regional performance analysis.

5️⃣ Dashboard Development
KPI cards.
Interactive filters.
Trend visualizations.
Business performance monitoring.

Key Performance Indicators (KPIs)
Total Revenue
Total Profit
Total Orders
Average Order Value
Profit Margin
Top Selling Product
Best Performing Category
Regional Revenue Contribution
Dashboard Features
Sales Analytics
Monthly Sales Trends
Revenue Growth Analysis
Seasonal Performance Tracking
Product Analytics
Top Selling Products
Category Performance
Product Profitability
Customer Analytics
Customer Segmentation
Repeat Customer Analysis
Purchase Behavior Insights
Regional Analytics
Region-wise Sales Distribution
Profit by Region
Market Performance Comparison
Sample Insights Generated
Identified highest revenue-generating product categories.
Determined regions contributing maximum profit.
Analyzed customer purchasing patterns.
Evaluated monthly sales growth trends.
Measured overall business performance using KPIs.

Repository Structure
Retail-Sales-Analytics-Dashboard
│
├── data
│   └── retail_sales.csv
│
├── notebooks
│   └── sales_analysis.ipynb
│
├── sql
│   └── sales_queries.sql
│
├── dashboard
│   └── retail_dashboard.pbix
│
├── images
│   └── dashboard_preview.png
│
├── requirements.txt
├── README.md
└── LICENSE
Dashboard Preview

{
	displayname = "Employees"
	success message = "Data Added Successfully!"
	Section
	(
		type = section
	 	row = 1
	 	column = 0   
		width = medium
	)
	employee_id
	(
    	type = autonumber
		displayname = "Employee ID"
		start index = 1
	 	row = 1
	 	column = 1   
		width = medium
	)
	full_name
	(
    	type = name
		displayname = "Full Name"
     	prefix
     	(
	     	 type = prefix
	     	 displayname ="Prefix"
	     	 visibility = false
	     	 value = {"Mr.","Mrs.","Ms."}
     	) 
     	first_name
     	(
	     	 type = first_name
	     	 displayname ="First Name"
     	) 
     	last_name
     	(
	     	 type = last_name
	     	 displayname ="Last Name"
	     	 visibility = false
     	) 
     	suffix
     	(
	     	 type = suffix
	     	 displayname ="Suffix"
	     	 visibility = false
     	) 
	 	row = 1
	 	column = 1   
		width = medium
	)
	job_title
	(
    	type = text
		displayname = "Job Title"
	 	row = 1
	 	column = 1   
		width = medium
	)
	department
	(
    	type = text
		displayname = "Department"
	 	row = 1
	 	column = 1   
		width = medium
	)
	hire_date
	(
    	type = date
		displayname = "Hire Date"
		alloweddays = 0,1,2,3,4,5,6
	 	row = 1
	 	column = 1   
		width = medium
	)
	email
	(
    	type = email
		displayname = "Email"
	 	row = 1
	 	column = 1   
		width = medium
	)
	phone
	(
    	type = phonenumber
		displayname = "Phone"
	 	row = 1
	 	column = 1   
		width = medium
	)
	manager
	(
    	type = text
		displayname = "Manager"
	 	row = 1
	 	column = 1   
		width = medium
	)
	
	actions
	{
		on add
		{
			submit
			(
   				type = submit
   				displayname = "Submit"
			)
			reset
			(
   				type = reset
   				displayname = "Reset"
			)
		}
		on edit
		{
			update
			(
   				type = submit
   				displayname = "Update"
			)
			cancel
			(
   				type = cancel
   				displayname = "Cancel"
			)
		}
	}
}


Clone the repository:

git clone https://github.com/yourusername/Retail-Sales-Analytics-Dashboard.git

Navigate to project folder:

cd Retail-Sales-Analytics-Dashboard

Install dependencies:

pip install -r requirements.txt
Business Value

This dashboard enables organizations to:

Monitor business performance efficiently.
Improve decision-making using data insights.
Identify profitable products and markets.
Enhance customer retention strategies.
Optimize sales and marketing efforts.
Skills Demonstrated
Data Cleaning
Exploratory Data Analysis (EDA)
SQL Querying
Data Visualization
Dashboard Development
Business Intelligence
Statistical Analysis
Reporting & Insights Generation
Future Enhancements
Sales Forecasting using Machine Learning
Customer Churn Prediction
Automated Reporting
Real-Time Data Integration
Cloud Deployment using AWS
Author
Vidya Shree L

Aspiring Data Analyst | Python | SQL | Power BI | Data Scienceform employees
