# Web Scraping and MongoDB Integration

This Python script showcases web scraping functionality using the `requests` library and data storage in MongoDB. It scrapes product details from a specific URL, processes the data with Beautiful Soup, conducts data cleaning, and integrates MongoDB for data storage and retrieval.
In this application, we are fetching data from the e-commerce website, which is known as eCRATER, however, the purpose of this website is to buy and sell antique things. To perform web scraping, BeatifulSoup library is being used. Furthermore, the BeatifulSoup library is beneficial for fetching records from HTML tags. Prior to storing records in Database, cleaning must be done to sepearte unnecessary things from the raw data. Mongo Db will be used for storing records and performing database operations such as read, insert, update, delete.

![website Image](https://github.com/roshan1960701/Web-Scraping-/blob/main/Screenshot%202023-12-29%20at%2021.18.31.png)

- **Flowchart**:
![flowchart](https://github.com/roshan1960701/Web-Scraping-/blob/main/diagram%20(1).svg)

## Overview

- **Web Scraping**:
  - Utilizes the `requests` library to fetch HTML content.
  - Employs Beautiful Soup for parsing and extracting data from HTML tags.
  - Cleans the data by extracting specific information like product names, prices, categories, and image links.

- **Data Manipulation**:
  - Cleans the extracted data, replacing the dollar sign in prices and formatting image links for display.

- **Analysis and Filtering**:
  - Filters products based on price ranges and specific categories.
  - Presents filtered data in tabular format with images.

- **MongoDB Integration**:
  - Establishes a connection to a MongoDB database using `pymongo`.
  - Creates and interacts with a collection named `product_detail`.
  - Inserts, retrieves, and deletes records in MongoDB based on various parameters.

## Instructions

1. **Dependencies**:
   - Ensure you have the necessary libraries installed: `requests`, `beautifulsoup4`, `pandas`, `pymongo`, `IPython`.

2. **Setup**:
   - Confirm MongoDB is installed and running.
   - Replace the MongoDB connection string in the script with your credentials.

3. **Execution**:
   - Run the Python script (`web_scraping_mongodb.py`).
   - The script will scrape product data, perform data operations, and interact with MongoDB.

4. **Functionalities**:
   - Filtering products by price ranges and categories.
   - Storing scraped data in MongoDB and performing various database operations.

5. **References**:
   - Includes helpful links used for web scraping, Beautiful Soup, and MongoDB integration.

## Notes

- Ensure a stable internet connection to fetch data from the specified URL.
- Modify the code as required for different web scraping needs or database operations.

