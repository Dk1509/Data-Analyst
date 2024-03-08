1. Sales Overview:

YTD Total Sales:

Formula: YTD Total Sales = TOTALYTD(SUM(Sales[SalesAmount]), 'Date'[Date])
MTD Total Sales:

Formula: MTD Total Sales = TOTALMTD(SUM(Sales[SalesAmount]), 'Date'[Date])
YOY Growth in Total Sales:

Formula: YOY Growth = DIVIDE(SUM(Sales[SalesAmount]) - CALCULATE(SUM(Sales[SalesAmount]), SAMEPERIODLASTYEAR('Date'[Date])), CALCULATE(SUM(Sales[SalesAmount]), SAMEPERIODLASTYEAR('Date'[Date])))
Difference (YTD vs. PTYD Sales):

Formula: Difference YTD vs PTYD = [YTD Total Sales] - CALCULATE([YTD Total Sales], DATEADD('Date'[Date], -1, YEAR))
2. Average Price Analysis:

YTD Average Price:

Formula: YTD Average Price = [YTD Total Sales] / [YTD Cars Sold]
MTD Average Price:

Formula: MTD Average Price = [MTD Total Sales] / [MTD Cars Sold]
YOY Growth in Average Price:

Formula: YOY Growth in Avg Price = DIVIDE([YTD Average Price] - CALCULATE([YTD Average Price], SAMEPERIODLASTYEAR('Date'[Date])), CALCULATE([YTD Average Price], SAMEPERIODLASTYEAR('Date'[Date])))
Difference (YTD vs. PTYD Average Price):

Formula: Difference YTD vs PTYD Avg Price = [YTD Average Price] - CALCULATE([YTD Average Price], DATEADD('Date'[Date], -1, YEAR))
3. Cars Sold Metrics:

YTD Cars Sold:

Formula: YTD Cars Sold = CALCULATE(SUM(Sales[CarsSold]), 'Date'[Date])
MTD Cars Sold:

Formula: MTD Cars Sold = CALCULATE(SUM(Sales[CarsSold]), DATESMTD('Date'[Date]))
YOY Growth in Cars Sold:

Formula: YOY Growth in Cars Sold = DIVIDE([YTD Cars Sold] - CALCULATE([YTD Cars Sold], SAMEPERIODLASTYEAR('Date'[Date])), CALCULATE([YTD Cars Sold], SAMEPERIODLASTYEAR('Date'[Date])))
Difference (YTD vs. PTYD Cars Sold):

Formula: Difference YTD vs PTYD Cars Sold = [YTD Cars Sold] - CALCULATE([YTD Cars Sold], DATEADD('Date'[Date], -1, YEAR))
📈 Problem Statement 2: Charts Requirement

1. YTD Sales Weekly Trend:

Formula: No specific formula. Utilizes a line chart with 'Weeks' on the X-axis and 'Total Sales Amount' on the Y-axis.
2. YTD Total Sales by Body Style:

Formula: Utilizes a Pie chart with 'Body Style' as the category and 'Total Sales Amount' as the values.
3. YTD Total Sales by Color:

Formula: Utilizes a Pie chart with 'Car Color' as the category and 'Total Sales Amount' as the values.
4. YTD Cars Sold by Dealer Region:

Formula: Utilizes a Map chart with 'Dealer Region' and 'Total Cars Sold' as data points.
5. Company-Wise Sales Trend in Grid Form:

Formula: Utilizes a table visualization with 'Company Name' and 'YTD Sales Figures' as columns.
6. Details Grid Showing All Car Sales Information:

Formula: Utilizes a detailed table showcasing various attributes like 'Car Model', 'Body Style', 'Color', 'Sales Amount', 'Dealer Region', 'Date', etc.
