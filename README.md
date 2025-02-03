# Yanki Ecommerce Data Pipeline

This project involves designing and implementing a **data pipeline** to clean, transform, and load raw e-commerce data into a structured PostgreSQL database. The pipeline ensures data integrity, normalization, and efficient storage for analysis and decision-making.

---

## Project Overview

The goal of this project is to process raw e-commerce data from Yanki Ecommerce, clean and transform it, and store it in a normalized relational database. The pipeline includes:

1. **Data Cleaning**: Handling missing values, splitting customer names, and converting data types.
2. **Data Transformation**: Creating normalized tables for customers, products, shipping, orders, and transactions.
3. **Database Design**: Building a PostgreSQL database with proper schema design and referential integrity.
4. **Data Loading**: Automating the ingestion of cleaned data into the database.

---

## Technologies Used

- **Programming Languages**: Python
- **Libraries**: Pandas, psycopg2
- **Database**: PostgreSQL
- **Tools**: Jupyter Notebook (for development), CSV files for data storage

---

## Project Structure

```
yanki-ecommerce-data-pipeline/
├── Dataset/
│ ├── raw_data/ # Raw e-commerce data
│ └── clean_data/ # Cleaned and transformed data
├── scripts/
│ ├── data_cleaning.py # Script for cleaning and transforming data
│ ├── database_creation.py # Script for creating the database and tables
│ └── data_loading.py # Script for loading data into the database
├── README.md # Project documentation
```

---

## Setup Instructions

### Prerequisites
1. Install [Python](https://www.python.org/downloads/) (version 3.8 or higher).
2. Install [PostgreSQL](https://www.postgresql.org/download/).
3. Clone this repository:
   ```bash
   git clone https://github.com/Joshuatolu/yanki-ecommerce-data-pipeline.git
4. Navigate to the project directory:
   ```bash
   cd yanki-ecommerce-data-pipeline

## Database Configuration
1. Create a PostgreSQL database named yanki.
2. Update the database connection parameters in the scripts/database_creation.py file.

## Running the Pipeline

### Data Cleaning:

Run the data_cleaning.py script to clean and transform the raw data
This will generate cleaned CSV files in the Dataset/clean_data/ folder.

### Database Creation:

Run the database_creation.py script to create the database schema and tables

### Data Loading:

Run the data_loading.py script to load the cleaned data into the database

## Database Schema
The database consists of the following tables:

CUSTOMER: Stores customer information (e.g., name, email, phone number).

PRODUCT: Stores product details (e.g., name, brand, category, price).

SHIPPING: Stores shipping information (e.g., address, city, state, country).

ORDER: Stores order details (e.g., customer ID, product ID, quantity, total price).

YANKI_TB: Stores transaction status for each order.

## Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes.
4. Submit a pull request.

## Contact
For questions or feedback, feel free to reach out:

**Name:** ONIBIYO Joshua Toluse

**Email:** toluseonibiyo@gmail.com

**GitHub:** [My GitHub Profile](https://github.com/Joshuatolu/)
