 # Chat-Assistant-for-SQLite-Database
This project is a Python-based chat assistant designed to interact with an SQLite database. The assistant can answer a variety of natural language queries related to employees and departments, making it a useful tool for managing company data.

## Overview
The chat assistant allows users to ask questions about employees and departments in a company. The assistant processes natural language queries, converts them into SQL commands, and fetches data from the SQLite database to provide meaningful responses.

## Features
* The assistant can handle queries like-
  - "Show me all employees in the Sales department."
  - "Who is the manager of the Engineering department?"
  - "List all employees hired after 2021-01-01."
  - "What is the total salary expense for the Marketing department?"

## Database Schema
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

## Setup and Installation
### Requirements
 * Python 3.12
 * SQLite3 Python library (comes preinstalled with Python)
 * Streamlit
 
## Installation Steps
* Install the required libraries:-
  - It’s recommended to use a virtual environment, but it’s not mandatory.
* Set up the SQLite database:-
  - database file ```company.db```
* Run the Streamlit app:-
  - simply run the command ```streamlit run app.py```
    
## How the Assistant Works
* User Query Input:
  The user inputs a query in natural language via the Streamlit interface. The assistant processes this input and tries to match it to a pre-defined set of query patterns.
* Query Processing:
  Once the input is received, the assistant uses simple NLP techniques or keyword matching to detect the type of query and convert it into a SQL query.
*  Displaying Results:
  The results are displayed in a user-friendly format in the Streamlit interface.
* Error Handling:
  If the query cannot be processed or if the department name is invalid, the assistant will respond with an appropriate error message. 




 


