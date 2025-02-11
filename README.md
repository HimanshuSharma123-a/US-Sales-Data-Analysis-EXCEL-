![ ](https://github.com/HimanshuSharma123-a/US-Sales-Data-Analysis-EXCEL-/blob/main/US.png)

# US Sales Data Analysis (Excel)
Complete Excel Project

A client has shared a sales dataset and seeks insights, including sales trends over time, state-wise sales comparison, monthly sales analysis, identifying top-profit customers, and evaluating product category performance.

## Author
HimanshuSharma123-a

## Table of Contents
- [Business Problem](#business-problem)
- [Data Source](#data-source)
- [Data Overview](#data-overview)
- [Method](#method)
- [Quick Glance At The Dashboard](#quick-glance-at-the-dashboard)
- [Data Cleaning and Manipulation](#data-cleaning-and-manipulation)
- [Dashboarding](#dashboarding)
- [Slicers](#slicers)

## Business Problem

### Business Problem Statement:
A client has provided their sales dataset and requested insights from the data, focusing on several factors such as changes in sales orders over the years, a comparison of sales data across different states, monthly sales volume analysis, identification of top-profit-generating customers, and an evaluation of the performance of various product categories.

## Data Source
- [US Store Sales Dataset](https://www.kaggle.com/datasets/saadharoon27/us-store-sales-dataset)

## Data Overview

| Column Name    | Description                                                                |
|----------------|----------------------------------------------------------------------------|
| Order Date     | Consists of the date on which a specific order was created                 |
| Customer Name  | Consists of the full name of the customer who created an order             |
| State          | Name of the state the customer belonged to                                 |
| Category       | Which category the ordered product belonged to                             |
| Sub-Category   | Name of the sub-category of the ordered product                            |
| Product Name   | Name of the ordered product                                                |
| Sales          | The price at which the product was sold                                    |
| Quantity       | Number of quantities the customer ordered of that product                  |
| Profit         | How much the firm made in that transaction                                 |

## Method
- Exploratory Data Analysis (EDA)

## Quick Glance At The Dashboard
![Dashboard Image](https://github.com/HimanshuSharma123-a/US-Sales-Data-Analysis-EXCEL-/blob/main/Glance.png) <!-- Insert the link to your dashboard image here -->
## THIS CHART CREATED WITH TEAM MEMBERS AND THE HELP OF YOUTUBE 
## Data Cleaning and Manipulation

To create efficient pivot tables and dashboards with the provided data, the initial step involved converting the data into a structured table named ‘SalesData’ using the "create table" option. This transformation enhances data organization, making it more conducive for effective analysis and visualization.

### Column Treatment and Adjustments:

1. **Sales Column**: The ‘Sales’ column was in a general format, which could have potentially caused issues when creating visual representations. To ensure smooth visual plotting, it was necessary to convert the values into a Number format.
2. **Quantity Column**: Similarly, the ‘Quantity’ column was adjusted to remove decimal places.
3. **Profit Column**: The ‘Profit’ column was also converted to a Number format.
4. **Order Date Column**: The 'Order Date' column was converted into a date format and subsequently organized in ascending order, ensuring chronological arrangement.
5. **Month Column**: A new column, 'Month', was added to enable data visualization in monthly terms using the TEXT() function to extract the month and display it in a user-friendly manner (‘mmm’ format).
6. **Year Column**: A new column, 'Year', was added to enable data visualization in yearly terms using the YEAR() function.

## Dashboarding

### SalesByCategory Sheet:
- Created a pivot table titled "SalesByCategory" to visually represent the sum of sales figures of different sub-categories.
- Inserted 'Sub-Category' in the rows field and 'Sales' in the Values field.
- Sorted the data in descending order by sales and created a funnel chart from the duplicated data.

### ProfitGainedOverTime Sheet:
- Generated a pivot table to create a line chart displaying profit trends over the years for categories: Furniture, Office Supplies, and Technology.
- Inserted 'Category' in the columns field, 'Year' in the rows field, and 'Sum of Profit' in the Values field.

### MonthlySales Sheet:
- Established a pivot table to generate an area chart representing the cumulative sales values for each month.
- Inserted 'Month' in the rows field and 'Sum of Values' in the Values field.
- Added a slicer to the 'Year' column to filter data for specific years.

### Top5Customers Sheet:
- Created a pivot table to visualize the top five customers generating the highest profits.
- Inserted 'Customer Name' in the Rows field and 'Sum of Profit' in the Values field.
- Created a pie chart to illustrate the contribution of these key customers.

### SalesByState Sheet:
- Created a pivot table titled "SalesByState" to visually represent the sum of sales by state.
- Inserted 'State' in the rows field and 'Sum of Values' in the Values field.
- Created a map chart from the duplicated data.

### CustomerCount Sheet:
- Copied 'Customer Name' and 'Year' columns to a new sheet (CustomerCount) and removed duplicates to count unique customers yearly.
- Created a pivot chart and used a bar chart to visualize the data.

## Slicers
- Added slicers based on product categories to allow easy filtering and analysis.
- Established connections between all slicers and visual elements to ensure seamless reflection of filters across all graphs.

