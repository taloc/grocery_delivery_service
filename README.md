# Grocery Delivery Service Dataset

## Overview
This repository contains a dataset for analyzing grocery delivery sales, designed to support historical and predictive analysis for a grocery delivery app. The dataset includes six tables capturing orders, products, aisles, departments, and related details. This data is ideal for creating Power BI reports, forecasting models, and validating predictions to inform app development decisions.

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

## Usage
This dataset is suitable for:
- Building Power BI dashboards to visualize historical sales trends and customer behavior
- Developing predictive models to forecast future orders
- Validating forecast accuracy by comparing predictions (using prior data) against training data
- Analyzing delivery patterns, product popularity, and reorder trends

## Download Instructions
The dataset is available in a zipped folder:  
[Download grocery_deliveries.zip](https://github.com/taloc/grocery_delivery_service/blob/main/grocery_deliveries.zip)

**Steps to Download:**
1. Navigate to the link above.
2. If you see: "Sorry about that, but we can’t show files that are this big right now," the data is still accessible.
3. Click the **Download raw file** button in the upper-right corner of the file preview.
4. Choose a save location on your device and click **Save**.

## Notes
- Ensure proper data cleaning and transformation before analysis, as the dataset may contain inconsistencies.
- For predictive modeling, use the `Order Products Prior` table for training and the `Order Products Train` table for validation.
- A separate file (PDF or Word) documenting any data cleaning or transformations is recommended when sharing analysis results.

## License
This dataset is provided for educational and analytical purposes. Please ensure compliance with any applicable data usage policies.

## Contact
For questions or contributions, please open an issue or submit a pull request on this repository.
