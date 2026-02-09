# ApexPlanet_Task1_DataWrangling
Data cleaning and feature engineering on Superstore retail dataset.


ApexPlanet Task-1: Data Immersion & Wrangling — Superstore Dataset
📌 Project Objective

The objective of this project is to clean and prepare a real-world retail sales dataset for downstream analytics.
This includes understanding the dataset structure, identifying data quality issues, performing cleaning operations, and engineering new features to make the data analysis-ready.

📊 Dataset Overview

Dataset Name: Superstore Retail Dataset

Rows: 9,800

Columns (after cleaning & feature engineering): 21

Domain: Retail Sales Analytics

The dataset contains order-level transaction details including customer information, product categories, shipping details, and revenue.

🔍 Data Quality Issues Identified

During exploration, the following issues were observed:

11 missing values in the Postal Code column

Postal Code stored as numeric although it represents a categorical identifier

Date fields initially stored as object/string format

Required validation for duplicate records

🧹 Data Cleaning Performed

The following cleaning steps were applied:

Converted Order Date and Ship Date to datetime format

Handled missing Postal Code values

Verified that no duplicate rows existed

Ensured consistent column datatypes across the dataset

⚙️ Feature Engineering

New analytical features were created:

Order Year – extracted from Order Date

Order Month – extracted from Order Date

Shipping Days – calculated as the difference between Ship Date and Order Date

These features enable time-series analysis and logistics performance evaluation.

📘 Data Dictionary
Column Name	Description	Data Type	Business Use
Row ID	Unique row identifier	int	internal indexing
Order ID	Unique order transaction code	object	track orders
Order Date	Date when order was placed	datetime	sales trends
Ship Date	Date when order was shipped	datetime	delivery analysis
Ship Mode	Shipping method used	object	logistics analysis
Customer ID	Unique customer identifier	object	customer tracking
Customer Name	Full customer name	object	customer segmentation
Segment	Customer category	object	segmentation
Country	Country of customer	object	geographic analysis
City	City of customer	object	regional performance
State	State of customer	object	regional analysis
Postal Code	ZIP / postal region (nullable)	category / string	location grouping
Region	Business region	object	regional KPIs
Product ID	Unique product code	object	product tracking
Category	Product category	object	category performance
Sub-Category	Product sub-category	object	detailed analysis
Product Name	Product description	object	product analytics
Sales	Revenue amount	float	revenue calculation
Order Year	Year extracted from Order Date	int	yearly trend
Order Month	Month extracted from Order Date	int	seasonality
Shipping Days	Days between order and shipment	int	logistics KPI
📂 Repository Structure
ApexPlanet_Task1_DataWrangling/
 ├── Cleaned Data CSV/
 │   └── Superstor_Cleaned_Task1.csv
 ├── notebook/
 │   └── task_1.ipynb
 └── README.md

📈 Key Learnings

Data exploration and profiling

Handling missing values and datatypes

Feature engineering for business analysis

Preparing datasets for analytics pipelines

Professional documentation using GitHub
