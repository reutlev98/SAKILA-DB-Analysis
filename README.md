# SAKILA-DB-Analysis

## Introduction
This project involves performing data analysis on the **SAKILA DB**, a sample relational database that contains data about a fictional DVD rental store. The project demonstrates SQL proficiency in data retrieval, filtering, joining tables, aggregation, pattern matching, and optimization techniques, as well as the use of Python for automating and analyzing the results.

## Part 1: SQL Queries

### Dataset Overview
The **SAKILA DB** contains multiple tables that represent different entities such as **films, actors, stores, staff, customers, rentals, payments**, and more. This real-world example provides a comprehensive dataset for practicing SQL querying skills, focusing on managing relationships and processing large datasets.


### Key SQL Techniques

1. **Data Retrieval and Filtering**:
   - Queries demonstrate how to extract relevant data using `SELECT` statements and `WHERE` clauses to filter results based on specific conditions.

2. **Joining Tables**:
   - SQL `JOIN` operations combine data from multiple related tables (e.g., **customers**, **rentals**, and **films**) to establish relationships and create more comprehensive result sets.

3. **Aggregation and Grouping**:
   - Queries use aggregate functions like `COUNT()`, `SUM()`, and `AVG()` to calculate summary statistics. `GROUP BY` is employed to group the results based on specific columns.

4. **Subqueries**:
   - Subqueries are used to perform complex data retrieval by nesting queries. They help in breaking down problems into smaller, more manageable queries.

5. **Pattern Matching**:
   - The `REGEXP_LIKE` function is used for pattern matching, enabling queries to search for specific formats or patterns in text fields, such as finding customers or movie titles based on certain conditions.

6. **Set Operations (UNION)**:
   - `UNION` merges the results from multiple queries, eliminating duplicates and combining data from different sources into a single result set.

---

## Part 2: Python Script

### Overview
The Python script is used to automate querying the **SAKILA DB**, process the results, and conduct further analysis using Python libraries such as `pandas`. The script enhances data manipulation capabilities and provides error handling mechanisms for smooth execution.

### Running the Script

To run the Python script, follow these steps:

1. **Install Dependencies**:
   - Ensure that you have the necessary libraries installed. You can install them using `pip`:
     ```bash
     pip install pandas mysql-connector-python
     ```

2. **Configure the Database Connection**:
   - Modify the script to include your database credentials:
     ```python
     import mysql.connector

     db_connection = mysql.connector.connect(
         host="localhost",
         user="your_username",
         password="your_password",
         database="sakila"
     )
     ```

3. **Run the Script**:
   - Execute the Python script to run predefined queries and analyze the data:
     ```bash
     python reviewer.py
     ```

### Usage
1. **Execution**:
   - Run the Python script `movie_rating_system.py`. Upon execution, the program will prompt you to enter your **ID**.
   
2. **New Reviewer**:
   - If you're a new reviewer, the system will ask for your **first name** and **last name**.
   
3. **Movie Rating**:
   - Once your information is entered, you can input the name of the movie you'd like to rate. If the movie exists in the database, you will be prompted to enter a rating for it.
   - If the movie has an existing rating, the program will update it. Otherwise, it will insert a new rating record.

4. **Displaying Ratings**:
   - After submitting your rating, the system will display all the movie ratings currently stored in the database.
  
   ![image](https://github.com/user-attachments/assets/5bf4f806-1e13-4992-93cf-6984fe7bbf18)


### Error Handling
- The script includes `try-except` blocks to manage:
  - Database connection errors.
  - SQL query errors.
  - Data processing errors (e.g., incorrect data types or missing fields).


## Conclusion
This project highlights the use of SQL for performing complex data operations on the **SAKILA DB** and the ability to automate and extend analysis through Python scripting. By optimizing query performance, handling errors, and ensuring data integrity, this project provides a solid example of effective data analysis practices in a relational database environment.

## Contributors
- Reut Lev (reutlev98)
- Ye'ela Granot (yeela8g)






