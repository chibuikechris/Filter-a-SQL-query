# Filter-a-SQL-query
### Applying basic filters to SQL queries to retrieve information from a MariaDB database
## Task 1. List all organization machines - In this task, we need to get a list of all organization machines and their operating systems. The data is contained in the machines table.
### Run a SQL query to retrieve only the device_id and operating_system columns from the machines table.
- SELECT device_id, operating_system
  FROM machines;
 <img width="430" height="142" alt="task 1" src="https://github.com/user-attachments/assets/326874e1-350c-4d2f-8d8a-2dcd7d666137" />


## Task 2. Retrieve a list of the machines with OS 2 - In this task, we need to obtain a list of all machines with the 'OS 2' operating system because these machines need an update.
### Select all the records from the machines table with a value of 'OS 2' in the operating_system column
- SELECT *
  FROM machines
  WHERE operating_system = 'OS 2';
<img width="432" height="157" alt="task 2" src="https://github.com/user-attachments/assets/68f25e19-a90e-486d-a7e4-eda4255f76a9" />

  
## Task 3. List employees in specific departments- In this task, you need to retrieve a list of all the employees in the Finance and Sales departments to obtain their office numbers.
- SELECT *
  FROM employees
  WHERE department ='Finance';
  <img width="439" height="215" alt="task 3" src="https://github.com/user-attachments/assets/26e99c1c-0c2b-4368-a4b0-c6cb0a627101" />

  
  - ### Modify the previous query so that it returns employees who are in the 'Sales' department
  - SELECT *
    FROM employees
    WHERE department ='Sales';
    <img width="433" height="189" alt="task 3b" src="https://github.com/user-attachments/assets/d0f62578-b3c6-4096-a221-dd94ab53be28" />


  - ## Task 4. Identify employee machines - In this task, we need to obtain certain employee and computer information
  - Write a query to identify which employee uses the office in 'South-109'. (The data must be returned from the office column in the employees table.)
  - SELECT *
    FROM employees
    WHERE office = 'South-109';
    <img width="440" height="132" alt="task4" src="https://github.com/user-attachments/assets/dcf8cd58-657d-4a3c-ad5f-938afb6e45db" />

 
### Modify the query you used in the previous step so that it returns information on all the employees in the 'South' building. Use the LIKE operator with % in this query.
- SELECT *
  FROM employees
  WHERE office LIKE 'South%';
  <img width="431" height="191" alt="task 4b" src="https://github.com/user-attachments/assets/622fa242-f2f4-4c32-be1b-9346fdc4483b" />
