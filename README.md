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

## 3. Error Handling
 The assistant is built to handle a variety of potential issues gracefully:

 * Invalid or Unknown Queries: If a query cannot be understood, the assistant responds with a default error message like "Sorry, I didn’t understand that query."
 * No Results Found: If no data matches the query ,the assistant provides a helpful message, such as "No employees found in the Sales department."

## 4. User Interaction Flow

  * The user interacts with the assistant by typing queries in natural language.
  * The assistant processes the query, generates an appropriate SQL statement, executes it against the database, and then formats the results into a user-friendly response.
  * Responses are displayed back to the user in a clear and readable format. If no results are found or if there’s an error, the assistant will inform the user accordingly.



