# Sales Forecasting for Stores and Products

## Project Overview
This project aims to forecast the total sales for every product in each store for the upcoming month using historical sales data. The dataset includes daily sales records, and the goal is to predict the monthly amount of products sold.

## Project Description
This project utilizes machine learning models to predict future sales based on historical sales data. The dynamic nature of the dataset, with changing shops and products each month, presents a unique challenge in building robust models that can handle these variations effectively.

## Data Description
The dataset contains the following fields:
- `shop_id`: Unique identifier of a shop.
- `item_id`: Unique identifier of a product.
- `item_cnt_day`: Number of products sold (daily sales).
- `item_price`: Current price of an item.
- `date`: Date in format dd/mm/yyyy.
- `date_block_num`: A consecutive month number (e.g., January 2013 is 0, February 2013 is 1, ..., October 2015 is 33).

### Sample Training Data
| date       | date_block_num | shop_id | item_id | item_price | item_cnt_day |
|------------|----------------|---------|---------|------------|--------------|
| 02.01.2013 | 0              | 59      | 22154   | 999.00     | 1.0          |
| 03.01.2013 | 0              | 25      | 2552    | 899.00     | 1.0          |
| 05.01.2013 | 0              | 25      | 2552    | 899.00     | -1.0         |
| 06.01.2013 | 0              | 25      | 2554    | 1709.05    | 1.0          |
| 15.01.2013 | 0              | 25      | 2555    | 1099.00    | 1.0          |

### Sample Test Data
| ID | shop_id | item_id |
|----|---------|---------|
| 0  | 0       | 5037    |
| 1  | 1       | 5320    |
| 2  | 2       | 5233    |
| 3  | 3       | 5232    |
| 4  | 4       | 5268    |
