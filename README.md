# Business Insights from Sales and Shipping Data Using Python

#### Project Goal: Data Preprocessing & Visualization using Python

#### Dataset: E-Cart.xlsx

## Objective

To analyze and preprocess a business dataset by cleaning, transforming, and visualizing key patterns related to product revenue, marketing performance, and shipping trends. 
The goal is to uncover insights for better decision-making in sales and logistics.

## Tools Used

Pandas – Data manipulation

NumPy – Numerical computations

Matplotlib – Custom visualizations

Seaborn – Advanced statistical plotting

Jupyter Notebook – Interactive development


## Data Preprocessing Steps

### Loading Data

Loaded Excel dataset using pandas.read_excel()

### Initial Inspection

Used .head(), .info(), and .describe() to understand structure and summary

## Handling Missing Data

Checked missing values using isnull().sum()

Filled missing entries using forward fill (method='ffill')

Filled missing numeric columns using (mean/median)

### Feature Engineering

Created SHIPPING_YEAR from date column using pd.to_datetime().dt.year

Extracted SHIPPING_DAY to identify weekly trends

## Visualizations with Captions

### 1. Product-wise Revenue from Orders

A horizontal bar chart showing revenue grouped by PRODUCT_NAME, sorted in descending order with a dark background for clarity.
Each bar includes its value, helping easily identify top-selling products.

### 2. Orders by Marketing Channels

A bar chart showing count of ORDER_IDs grouped by MARKETING_CHANNEL, useful to evaluate the effectiveness of each channel in driving orders.

### 3. Weekly Shipping Pattern (2019–2021)

A line chart showing order frequency by day of the week (Monday to Sunday). The plot highlights which days are busiest for shipping across all years, supporting operations planning.

### 4. Yearly Order Volume Trends

A line graph showing total orders per year from 2019 to 2021. Useful to understand year-over-year performance and growth.

### 5. Orders Shipped by Year (Count Plot)

A simple bar chart showing the count of shipped orders per year. Helps in quickly comparing volume over time.

## Key Insights

A few products dominate revenue, indicating key performers
Certain marketing channels drive significantly more orders
Mid-week days (especially Wednesday) show peak shipping activity
There’s a clear upward trend in order volume from 2019 to 2021

## Conclusion
The dataset has been effectively cleaned and visualized. 
Using dark-themed, well-labeled plots, key insights around product performance, marketing effectiveness, and operational timing were uncovered. 
The data is now ready for predictive modeling, business intelligence dashboards, or further exploratory work.
