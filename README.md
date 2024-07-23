<h2 align = "center"> 1. DataBase </h2>

### 1. Create a Database and Table for Employees
CREATE TABLE employees (
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    role TEXT NOT NULL,
    salary REAL NOT NULL,
    age INTEGER NOT NULL,
    address TEXT NOT NULL,
    phone TEXT NOT NULL
);

### 2. Add a New Employee with All Details

INSERT INTO employees (id, name, role, salary, age, address, phone) 
VALUES (100, 'Fenish Patel', 'Student', 10000, 18, '123 xyz', '6353600958');

### 3. Add Multiple Employees with Selective Data

INSERT INTO employees (name, role, salary, age, address, phone) 
VALUES 
('Fenish Patel', 'Student', 10000, 18, '123 xyz ', '6353600958'),
('Darshan', 'Student', 10000, 18, '123 xyz', '6353600958');

### 4. Retrieve All Employee Information

SELECT * FROM employees;

### 5. Get Specific Columns for All Employees (e.g., name, salary)

SELECT name, salary FROM employees;

### 6. Find Employees with a Specific Role (e.g., Manager)

SELECT * FROM employees WHERE role = 'Manager';

### 7. Search for Employees with Names Containing "An" (Case-Insensitive)

SELECT * FROM employees WHERE name LIKE '%An%' COLLATE NOCASE;

### 8. Find Employees Older than 30 and Earning More than $70,000

SELECT * FROM employees WHERE age > 30 AND salary > 70000;

### 9. Change the Salary of an Employee with ID 100

UPDATE employe SET salary = 10000 WHERE id = 1;

### 10. Update the Address for Employees in the 'Sales' Role

UPDATE employees SET address = 'New Sales Office, Springfield' WHERE role = 'Sales';

### 11. Remove an Employee with ID 101

DELETE FROM employees WHERE id = 1;

### 12. Delete All Employees with Age Less than 20

DELETE FROM employees WHERE age < 20;
