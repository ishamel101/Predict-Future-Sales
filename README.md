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

### The final result for Date_Block_Num 34:(20 simple)

| ID | shop_id | item_id | date_block_num | item_cnt_month |
|----|---------|---------|----------------|----------------|
| 33847 | 10 | 13110 | 34 | 1.0 |
| 116645 | 49 | 19996 | 34 | 1.0 |
| 130864 | 47 | 16000 | 34 | 5.0 |
| 3289 | 5 | 13698 | 34 | 0.0 |
| 101312 | 19 | 6957 | 34 | 2.0 |
| 118637 | 53 | 1557 | 34 | 0.0 |
| 119803 | 53 | 3987 | 34 | 0.0 |
| 197897 | 41 | 18916 | 34 | 0.0 |
| 112040 | 50 | 5010 | 34 | 0.0 |
| 96538 | 14 | 22035 | 34 | 20.0 |
| 81162 | 15 | 4191 | 34 | 1.0 |
| 143718 | 58 | 21881 | 34 | 20.0 |
| 138361 | 57 | 4102 | 34 | 3.0 |
| 22953 | 2 | 6847 | 34 | 0.0 |
| 145965 | 58 | 20717 | 34 | 20.0 |
| 197746 | 41 | 5014 | 34 | 0.0 |
| 59724 | 25 | 8260 | 34 | 2.0 |
| 193317 | 46 | 3418 | 34 | 6.0 |
| 197171 | 41 | 15849 | 34 | 0.0 |
| 36283 | 12 | 1299 | 34 | 20.0 |
