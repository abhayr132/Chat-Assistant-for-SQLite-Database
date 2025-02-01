# Chat-Assistant-for-SQLite-Database

The chat assistant is designed to interact with an SQLite database and respond to natural language queries 
about employee and department data.

## 1.SQLite Database Setup
  The assistant relies on a small SQLite database with two tables:-
  
  1. Employees: This table stores employee details, including:
      - ID: A unique identifier for each employee.
      - Name: The name of the employee.
      - Department: The department to which the employee belongs.
      - Salary: The salary of the employee.
      - Hire_Date: The date when the employee was hired.

   2. Departments: This table stores information about the company's departments, including:
      - ID: A unique identifier for each department.
      - Name: The name of the department.
      - Manager: The name of the manager who oversees the department.

## 2. Query Handling
  The core functionality of the assistant is to convert user queries into SQL statements and fetch relevant data from the database.

  * The assistant accepts queries in natural language, such as:
    - "Show me all employees in the Sales department."
    - "Who is the manager of the Engineering department?"
    - "List all employees hired after 2021-01-01."
    - "What is the total salary expense for the Marketing department?"
 * The assistant uses basic string matching and regular expressions to extract the necessary information from the user’s query.
 for example-
    - It recognizes when a query is asking for employees in a specific department.
    - It matched the department name or date when needed.
 * Based on the information, the assistant constructs an SQL query to fetch the relevant data from the database.


