# PySpark Products & Categories

This project demonstrates how to join product and category data using PySpark, showing both products with categories with sorting and products without categories at the end.

## Data Structure

The example uses three main DataFrames:

### Products DataFrame
- `product_id`: Unique identifier for each product
- `product_name`: Name of the product

### Categories DataFrame
- `category_id`: Unique identifier for each category
- `category_name`: Name of the category

### Product-Category Relationship DataFrame
- `product_id`: Links to products
- `category_id`: Links to categories

## Expected Output on Example

```
+------------+-------------+
|product_name|category_name|
+------------+-------------+
|     AirPods|  Accessories|
|      iPhone|  Accessories|
|     MacBook|    Computers|
|        iPad|  Electronics|
|      iPhone|  Electronics|
|     Sticker|         NULL|
|   Trash Can|         NULL|
+------------+-------------+
```

## Usage

1. **Install Dependencies**:
   ```bash
   poetry install --no-root
   ```
   or
   ```bash
   poetry install --no-root --only main
   ```
   if don't need tests and jupyter server.

2. **Install JDK 17, f.e. on Debian**:
   ```bash
   sudo apt install openjdk-17-jdk-headless
   ```

3. **Run the Jupyter server if needed**:
   ```bash
   poetry run jupyter lab
   ```


## Requirements

- Python >= 3.11
- Poetry (for dependency management)
