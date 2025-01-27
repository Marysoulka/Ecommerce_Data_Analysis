# Ecommerce Data Analysis

## Project Overview
This project analyzes an extensive e-commerce dataset to uncover meaningful insights and trends. The analysis focuses on understanding customer behavior, sales trends, and relationships between key metrics such as discounts, quantity ordered, and revenue.

## Dataset
The dataset used for this project was sourced from [Kaggle](https://www.kaggle.com/datasets/zusmani/pakistans-largest-ecommerce-dataset/data). It contains detailed information about online trade orders from March 2016 to August 2018.

**Key Columns in the Dataset**:
- `order_status`: Status of the order (e.g., completed, canceled, refunded).
- `payment_method`: Method used for payment (e.g., credit card, cash).
- `category_name`: Product category.
- `grand_total`: Total revenue for an order.
- `quantity_ordered`: Number of items ordered.
- `discount_amount`: Discount applied to an order.
- `market_value`: Market value of the order.

## Steps in the Analysis

### 1. **Data Cleaning and Preparation**
- Removed unnecessary columns (`Unnamed` columns, `M-Y`).
- Handled missing values using the mode (most frequent value).
- Fixed data types for numeric and date fields.
- Replaced invalid values in categorical columns (e.g., `\N`, `#REF!`) with `NaN`.

### 2. **Exploratory Data Analysis (EDA)**
**Key Insights from EDA**:
1. **Category Analysis**:
   - The category generating the highest revenue (`grand_total`) is `Women's Fashion`.
   - The category with the highest number of orders (`quantity_ordered`) is `Mobiles & Tablets`.
2. **Order Status vs. Payment Method**:
   - Visualized the relationship between `order_status` and `payment_method` using a heatmap.
3. **Top Customers**:
   - Identified the top 10 customers with the highest number of orders.
4. **Discount Analysis**:
   - Analyzed the relationship between `discount_amount` and `quantity_ordered` to understand the impact of discounts on sales.
5. **Trends Over Time**:
   - Monthly sales trends for top-performing categories (`Top 5 Categories`).
6. **Price vs. Grand Total Check**:
   - Highlighted discrepancies where `grand_total` is greater than `price`, potentially indicating multi-item orders or high-value items.

### 3. **Visualizations**
The following charts were created to enhance the analysis:
1. **Bar Chart**: Total sales (grand total) by category.
2. **Line Plot**: Trends for quantity ordered in top 5 categories over time.
3. **Scatter Plot**: Relationship between discount amount and quantity ordered.
4. **Bar Chart**: Top 10 customers by total orders.
5. **Bar Chart**: Distribution of total orders across all customers.

## Results
Key insights derived from the analysis:
- `Women's Fashion` contributes significantly to total revenue, but `Mobiles & Tablets` lead in order volume.
- Customers prefer `Cash on Delivery (COD)` across most categories.
- Discounts positively correlate with higher sales volume for certain categories.
- Top customers contribute significantly to order volume, highlighting customer segmentation opportunities.

## Tools Used
- **Python**: For data cleaning, analysis, and visualizations.
- **Pandas**: Data manipulation and cleaning.
- **Matplotlib & Seaborn**: Data visualization.
- **Jupyter Notebook**: Interactive code development.







