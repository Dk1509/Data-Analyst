# Car Sales Dashboard Project

## Background
Our dynamic and thriving car dealership recognizes the pivotal role of efficient sales tracking and analysis in driving success. To enhance this process, we are embarking on a project to develop a robust and interactive Car Sales Dashboard using Power BI. This dashboard will act as a centralized hub for visualizing Key Performance Indicators (KPIs) related to our car sales, empowering data-driven decision-making.

## Objective
The primary objective of this project is to design and implement a comprehensive Car Sales Dashboard using Power BI. This dashboard will offer real-time insights into our sales data, providing a holistic view of our performance over time. By identifying trends and monitoring progress, we aim to make strategic decisions for sustainable growth.

## Problem Statement 1: KPI’s Requirement
The dashboard will incorporate the following key performance indicators:

### Sales Overview:
- Year-to-Date (YTD) Total Sales
- Month-to-Date (MTD) Total Sales
- Year-over-Year (YOY) Growth in Total Sales
- Difference between YTD Sales and Previous Year-to-Date (PTYD) Sales

### Average Price Analysis:
- YTD Average Price
- MTD Average Price
- YOY Growth in Average Price
- Difference between YTD Average Price and PTYD Average Price

### Cars Sold Metrics:
- YTD Cars Sold
- MTD Cars Sold
- YOY Growth in Cars Sold
- Difference between YTD Cars Sold and PTYD Cars Sold

## Problem Statement 2: Charts Requirement
1. **YTD Sales Weekly Trend:**
   - Display a line chart illustrating the weekly trend of YTD sales. X-axis represents weeks, and Y-axis shows the total sales amount.

2. **YTD Total Sales by Body Style:**
   - Visualize the distribution of YTD total sales across different car body styles using a Pie chart.

3. **YTD Total Sales by Color:**
   - Present the contribution of various car colors to the YTD total sales through a pie chart.

4. **YTD Cars Sold by Dealer Region:**
   - Showcase the YTD sales data based on different dealer regions using a map chart to visualize the sales distribution geographically.

5. **Company-Wise Sales Trend in Grid Form:**
   - Provide a tabular grid that displays the sales trend for each company, showcasing the company name along with their YTD sales figures.

6. **Details Grid Showing All Car Sales Information:**
   - Create a detailed grid presenting all relevant information for each car sale, including car model, body style, color, sales amount, dealer region, date, etc.

## Getting Started
To explore and deploy the Car Sales Dashboard, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/car-sales-dashboard.git
2 **Navigate to project directory.**
cd car-sales-dashboard

**Formula Used**
YTD Total Sales = SUM(Sales[SalesAmount])
Month-to-Date (MTD) Total Sales:MTD Total Sales = TOTALMTD(SUM(Sales[SalesAmount]), 'Date'[Date])

Year-over-Year (YOY) Growth in Total Sales:
YOY Growth = (YTD Total Sales - PTYD Total Sales) / PTYD Total Sales

Difference between YTD Sales and Previous Year-to-Date (PTYD) Sales:
Sales Difference = YTD Total Sales - PTYD Total Sales

**Average Price Analysis**:

**YTD Average Price**:
YTD Average Price = DIVIDE(YTD Total Sales, YTD Cars Sold)

**MTD Average Price**:
MTD Average Price = DIVIDE(MTD Total Sales, MTD Cars Sold)

**YOY Growth in Average Price**:

YOY Avg. Price Growth = (YTD Average Price - PTYD Average Price) / PTYD Average Price

**Difference between YTD Average Price and PTYD Average Price**:


Avg. Price Difference = YTD Average Price - PTYD Average Price

**Cars Sold Metrics**:
YTD Cars Sold:

YTD Cars Sold = COUNTROWS(Sales)
**MTD Cars Sold**:


MTD Cars Sold = COUNTROWS(FILTER(Sales, 'Date'[Date] <= MAX('Date'[Date])))

**YOY Growth in Cars Sold**:

YOY Cars Sold Growth = (YTD Cars Sold - PTYD Cars Sold) / PTYD Cars Sold

**Difference between YTD Cars Sold and PTYD Cars Sold**:


Cars Sold Difference = YTD Cars Sold - PTYD Cars Sold

3 **Open Power BI**:

Launch Power BI and open the project file (car_sales_dashboard.pbix).

4 **Explore the Dashboard**:

Interact with the different visuals and charts to gain insights into our car sales performance.
