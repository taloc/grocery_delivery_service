# Grocery Delivery Service Dataset

## Overview
This repository contains a dataset for analyzing grocery delivery sales, designed to support historical and predictive analysis for a grocery delivery app. The dataset includes six tables capturing orders, products, aisles, departments, and related details. 

- **Historical Orders Analysis**: Analyze historical sales data to identify trends, customer behavior, and other patterns using interactive Power BI visualizations.
- **Predictive Model**: Develop a forecast model with prior sales data and validate its accuracy against training data, presenting results in a dynamic Power BI dashboard.

## Dataset Description
The dataset consists of six tables, detailed below:

### Aisles Table
| Column    | Description                     |
|-----------|---------------------------------|
| aisle_id  | Unique identifier for each aisle |
| aisle     | Name of the aisle              |

### Departments Table
| Column        | Description                         |
|---------------|-------------------------------------|
| department_id | Unique identifier for each department |
| department    | Name of the department             |

### Order Products Prior Table
| Column            | Description                                      |
|-------------------|--------------------------------------------------|
| order_id          | Unique identifier for each order                 |
| product_id        | Unique identifier for each product               |
| add_to_cart_order | Order in which the product was added to the cart |
| reordered         | Binary indicator (1 = reordered, 0 = not reordered) |

### Order Products Train Table
| Column            | Description                                      |
|-------------------|--------------------------------------------------|
| order_id          | Unique identifier for each order                 |
| product_id        | Unique identifier for each product               |
| add_to_cart_order | Order in which the product was added to the cart |
| reordered         | Binary indicator (1 = reordered, 0 = not reordered) |

### Orders Table
| Column                   | Description                                  |
|--------------------------|----------------------------------------------|
| order_id                 | Unique identifier for each order             |
| user_id                  | Unique identifier for each user              |
| eval_set                 | Dataset category (prior, train, or test)     |
| order_number             | Sequence number of the order for the user    |
| order_dow                | Day of the week the order was placed (0-6, where 0 = Sunday) |
| order_hour_of_day        | Hour of the day the order was placed (0-23)  |
| days_since_prior_order   | Days since the user’s previous order         |

### Products Table
| Column        | Description                              |
|---------------|------------------------------------------|
| product_id    | Unique identifier for each product       |
| product_name  | Name of the product                     |
| aisle_id      | Identifier linking to the aisles table   |
| department_id | Identifier linking to the departments table |



## Notes

- This dataset is sourced from the Instacart Market Basket Analysis dataset [Instacart Market Basket Analysis](https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis/data?utm_source=chatgpt.com&select=products.csv).
- Due to privacy concerns, the dataset is a subset sample and does not contain sensitive information.


## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
