###
Project Overview:

![image](https://github.com/921zheng/pyspark_tandoori_project/assets/139349595/d2a830ba-7575-4b71-9afb-33230ad2fed3)

### 
Kanban link : https://lihong.kanbantool.com/b/1047651#?

###
Introduction:
The project "pyspark_tandoori_project" deals with analyzing sales and price data from two restaurants. The dataset consists of four CSV files, two containing sales information and the other two containing price information for each restaurant. The sales dataset includes columns such as 'Order Number', 'Order Date', 'Item Name', 'Quantity', 'Product Price', and 'Total products'. Meanwhile, the price dataset includes columns for 'Item Name' and 'Product Price'. The project aims to address four key questions related to the performance and characteristics of the two restaurants.

### 
Goal:
The goal of the project is to leverage PySpark for data analysis to extract valuable insights that can inform strategic decision-making and drive business growth for the two restaurants.

###
Process:
1. Analysis of Total Sales by Year:
The initial step involves filtering out rows with empty 'Quantity' cells, as they were added manually. Then, a new column called 'Year' is created by extracting the year from the 'Order Date'. Additionally, a 'Total Price for each item' column is added by multiplying the 'Quantity' and 'Product Price' columns. The total sales for each year are calculated using groupby and orderBy operations. Finally, a line chart is created to visualize the sales trend of both restaurants over the years.

2. Determining the Most Frequently Ordered Items:
To identify the most frequently ordered items, a new column called 'Quantity Sum' is created by summing up the quantities for each item. The most ordered items for each year are determined by assigning ranks to items based on their frequency of orders. The DataFrame is then filtered to retain only the top-ranked items for each year.

3. Analysis of Item Contributions to Sales in 2018:
Given that both restaurants achieved their highest sales in 2018, the analysis focuses on this year. The data for 2018 is filtered, and the sum of sales for each item is calculated. The top five items contributing the most to sales are identified and visualized using a bar chart.

4. Comparison of Average Item Prices and Item Numbers:
The average item prices and the number of items for each restaurant are compared. The average item price and the total number of items are calculated for each restaurant.

5. Determining the Busiest season:
Leveraging the 'Order Date', we've derived 'Month' and 'Season' columns. The aggregate sales volume per season, calculated as the cumulative "Total Price for each item", provides a comprehensive view of seasonal performance.

###
Results:
Both restaurants experienced a growth in sales from 2015 to 2018, with the second restaurant exhibiting a faster growth rate. However, sales for both restaurants declined significantly in 2019.

Plain Papadum emerged as the most frequently ordered item across all years, indicating its popularity among customers.

In 2018, Chicken Tikka Masala, Pilau Rice, and Korma - Chicken were among the top-selling items for the first restaurant, while Bombay Aloo and Chicken Tikka (Main) were among the top-selling items for the second restaurant.

The second restaurant had a higher average item price and a slightly larger number of items compared to the first restaurant.

The first restaurant experiences its peak activity during the vibrant season of Spring, while the second restaurant thrives amidst the wintry charm of Winter, marking it as their busiest period.

###
Improvement:
Prioritize basic analyses at the outset, such as the comparison of average item prices and item numbers, to provide a clearer structure to the project.
Enhance code readability and clarity by segregating analyses for each restaurant and providing clearer documentation for each step to improve the overall organization and understanding of the project.

   
