Python PDF Report Automation for Superstore Sales
Project Overview
This project demonstrates a complete, end-to-end data analysis workflow built in Python. The primary goal was to create an automated tool that reads raw sales data, performs a comprehensive analysis, generates key business visualizations, and compiles all findings into a professional, multi-page PDF report.

This showcases skills in data cleaning, exploratory data analysis (EDA), time-series forecasting, and report automation, simulating a common real-world task for a data analyst.

Final Product: The script generates a file named Sales_Report.pdf.

Tools & Libraries:

Python

Pandas: For data loading, cleaning, and manipulation.

Matplotlib & Seaborn: For creating data visualizations.

Statsmodels: For building the SARIMA time-series forecasting model.

FPDF2: For programmatically generating the final PDF report.

Jupyter Notebook: As the development environment.

Analysis & Visualization Steps
The Python script performs the following analytical steps:

1. Data Loading and Preparation
The superstore_sales.csv dataset is loaded into a Pandas DataFrame. The date columns are converted to the proper datetime format to enable time-based analysis, and the data is checked for missing values.

2. Exploratory Data Analysis (EDA)
To understand the business performance, several key questions were answered:

Overall Sales Trend: A line chart was created to visualize sales performance over the entire period, identifying seasonal patterns and overall growth.

Top Product Categories: A bar chart was generated to identify the top 10 best-selling product sub-categories, highlighting the most important revenue drivers.

Customer & Regional Performance: Bar charts were created to analyze sales by customer segment (Consumer, Corporate, Home Office) and by geographical region.

3. Sales Forecasting
A predictive model was built to forecast sales for the next 12 months.

A SARIMA (Seasonal AutoRegressive Integrated Moving Average) model was chosen due to the clear seasonality present in the sales data.

The model was trained on the historical monthly sales data.

A forecast was generated, complete with a confidence interval, and visualized on a line chart comparing historical data to the prediction.

4. Automated PDF Report Generation
The final step uses the fpdf2 library to compile all findings into a single, clean report. The script programmatically:

Creates a custom PDF document with headers and footers.

Adds a title page and a written executive summary.

Inserts the previously generated charts (sales_trend.png, category_sales.png, forecast.png) into the document.

Saves the final output as Sales_Report.pdf.

How to Run This Project
Ensure you have Python and the required libraries installed (pandas, matplotlib, seaborn, statsmodels, fpdf2).

Place the train.csv file in the same directory as the Jupyter Notebook.

Run all the cells in the notebook from top to bottom.

The script will generate the chart images and the final Sales_Report.pdf in the project directory.
