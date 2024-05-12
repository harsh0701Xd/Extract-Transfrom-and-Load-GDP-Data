# ETL Project: Extract, Transform, and Load GDP Data

## Overview
This project involves creating an automated script to extract GDP data from a website, transform it into a desired format, and load it into both a CSV file and a SQLite database. The extracted data is then queried to display only entries with GDPs exceeding $100 billion USD. The entire process is logged for monitoring and documentation purposes.

## Project Structure
The project consists of the following main components:
1. **Preliminary Setup**: Installation of required libraries and initialization of known values.
2. **Data Extraction**: Extraction of GDP data from a specified URL using web scraping techniques.
3. **Data Transformation**: Conversion of GDP values from millions to billions and rounding to two decimal places.
4. **Data Loading**: Saving the transformed data into both a CSV file and a SQLite database.
5. **Querying Database**: Running a query on the database to filter entries with GDPs over $100 billion USD.
6. **Logging Progress**: Logging the progress of the code execution with timestamps.

## Code Structure
The code is organized into functions to perform specific tasks:

```python
def extract(url, table_attribs):
    '''Extracts data from the specified URL and returns a DataFrame.'''

def transform(df):
    '''Transforms the extracted data to meet the project requirements.'''

def load_to_csv(df, csv_path):
    '''Saves the transformed data to a CSV file.'''

def load_to_db(df, sql_connection, table_name):
    '''Loads the transformed data into a SQLite database.'''

def run_query(query_statement, sql_connection):
    '''Executes a query on the database table.'''

def log_progress(message):
    '''Logs progress messages with timestamps to a log file.'''
