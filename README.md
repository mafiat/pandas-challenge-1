# Wholesale Data Analysis Code

This Jupyter Notebook helps explore a dataset from a fictional e-commerce company, exploring and analyzing data to address real-world business questions. We will identify top customers, popular product categories, calculate profits, and more. We dempnstrate data exploration, transformation, and analysis. 

## Part 1: Explore the Data

In this part, we import the data and use Pandas to learn more about the dataset.

1. **Import the data** from the CSV file.
2. **View the column names**.
3. **Use the `describe` function** to gather some basic statistics.

### We get answers to the following questions using Pandas:
- What three item categories had the most entries?
- For the category with the most entries, which subcategory had the most entries?
- Which five clients had the most entries in the data?
- We store the client IDs of those top 5 clients in a list.
- How many total units (the `qty` column) did the client with the most entries order?

## Part 2: Transform the Data

Now that we have a better understanding of the data, we will transform the data for better and easier analysis.

1. Create a column that calculates the subtotal for each line using the `unit_price` and the `qty`.
2. Create a column for shipping price. Assume a shipping price of $7 per pound for orders over 50 pounds and $10 per pound for items 50 pounds or under.
3. Create a column for the total price using the subtotal and the shipping price along with a sales tax of 9.25%.
4. Create a column for the cost of each line using `unit_cost`, `qty`, and shipping price (assume the shipping cost is exactly what is charged to the client).
5. Create a column for the profit of each line using line cost and line price.

## Part 3: We do Data Validation

After transforming data, we will verify the results. You have email receipts showing the total prices for 3 orders:

- Order ID 2742071 had a total price of $152,811.89
- Order ID 2173913 had a total price of $162,388.71
- Order ID 6128929 had a total price of $923,441.25


## Part 4: Summarize and Analyze

Using the new columns with confirmed values, we will look for the following information:

1. How much did each of the top 5 clients by quantity spend? 

2. Create a summary DataFrame showing the totals for the top 5 clients with the following information: total units purchased, total shipping price, total revenue, and total profit.

3. Create a function to change the currency to millions of dollars. Format the data and rename the columns to names suitable for presentation. Then, sort the DataFrame in descending order by total profits.

4. We wrote 2-3 paragraphs summarizing our conclusions.

## Conclusion

The **Client ID 24741** is by far the most important customer, in Total Units Purchases, Total Revenues, and Total Profits, with **239,862 units purchased**, **M$82.27 in Revenues** and **M$36.58M in Profits** respectively. But it is interesting to note that it was not the customer with the highest number of entries.

**Client ID 38378** followed in 2nd with best Total Revenue of **M$12.91** and Total Profit of **M$3.27** while falling slightly short on Total Number of Units at **73,667 units purchased**.

