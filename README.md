# Retail Sales Data Analysis

## Project overview
This beginner-friendly Data Analytics project analyzes a sample retail store's sales data from 2024–2025. It uses **Python (Pandas), SQL, Excel, and Power BI** to understand revenue, profit, product performance, regional performance, and sales-channel trends.

> Dataset note: `data/retail_sales.csv` is synthetic sample data created for learning and portfolio practice. It is not real company data.

## Business questions
1. What are the total revenue, profit, orders, and units sold?
2. Which products generate the highest revenue and profit?
3. Which region performs best?
4. How do revenue and profit change month by month?
5. Which sales channel performs better: Online or Store?

## Repository structure
```text
Retail_Sales_Analytics_Project/
├── data/
│   └── retail_sales.csv
├── python/
│   └── analysis.py
├── sql/
│   └── analysis_queries.sql
├── outputs/                 # created when the Python script runs
├── powerbi/
│   └── dashboard_instructions.md
├── requirements.txt
└── README.md
```

## Tools
- Excel: data inspection, filters, PivotTables, charts
- Python: Pandas, data quality checks, aggregation
- SQL: business questions using GROUP BY and aggregate functions
- Power BI: interactive dashboard and DAX measures

## Run the Python analysis
1. Install Python 3.10+.
2. Open a terminal in the project folder.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run:
   ```bash
   python python/analysis.py
   ```
5. Check the generated `outputs/` folder for KPI, monthly, product, and region summaries.

## Excel analysis
Open `data/retail_sales.csv` in Excel. Convert the data to a table (`Ctrl + T`), then create PivotTables:
- Rows: `Product`; Values: Sum of `Revenue`, Sum of `Profit`
- Rows: `Region`; Values: Sum of `Revenue`
- Rows: `Sales_Channel`; Values: Sum of `Revenue`
- Rows: `Order_Date` grouped by Month and Year; Values: Sum of `Revenue`

## Open the dashboard
Double-click `dashboard.html` to open the ready-made interactive dashboard in Chrome/Edge. It includes KPI cards and charts with Category and Sales Channel filters. No installation is required.

## Power BI dashboard
For a native Power BI report, follow `powerbi/dashboard_instructions.md` and save your report as `powerbi/retail_sales_dashboard.pbix` from Power BI Desktop. Import `data/retail_sales.csv` using **Get Data → Text/CSV**.

## Key insights to write after running
Use your actual output files/dashboard to write 3–5 findings. Example format:
- The highest-revenue product was ______.
- The top-performing region was ______.
- The Online channel generated ______ compared with Store.
- Revenue was highest in ______.
Do not fill these with guesses; use your calculated results.

## GitHub upload
1. Create a new GitHub repository named `retail-sales-data-analysis`.
2. Keep it **Public** if you want recruiters to view it.
3. Upload the project folder, or run these commands from the project folder:
   ```bash
   git init
   git add .
   git commit -m "Add retail sales data analytics project"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/retail-sales-data-analysis.git
   git push -u origin main
   ```
4. Replace `YOUR-USERNAME` with your GitHub username.

## Resume bullet
Built a Retail Sales Data Analysis project using Python (Pandas), SQL, Excel, and Power BI to clean and analyze 1,200 sales records, track revenue and profit KPIs, and compare product, region, and sales-channel performance.
