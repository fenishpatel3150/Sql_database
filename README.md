<h2 align = "center"> 1. DataBase </h2>

### 1. Create a Database and Table for Employes`
```sql
CREATE TABLE employes (
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    role TEXT NOT NULL,
    salary REAL NOT NULL,
    age INTEGER NOT NULL,
    address TEXT NOT NULL,
    phone TEXT NOT NULL
);
```
### 2. Add a New Employe with All Details
```sql
INSERT INTO employes (id, name, role, salary, age, address, phone) 
VALUES (100, 'Fenish Patel', 'Student', 10000, 18, '123 xyz', '6353600958');
```
### 3. Add Multiple Employes with Selective Data
```sql
INSERT INTO employes (name, role, salary, age, address, phone) 
VALUES 
('Fenish Patel', 'Student', 10000, 18, '123 xyz ', '6353600958'),
('Darshan', 'Student', 10000, 18, '123 xyz', '6353600958');
```
### 4. Retrieve All Employe Information
```sql
SELECT * FROM employes;
```
### 5. Get Specific Columns for All Employees (e.g., name, salary)
```sql
SELECT name, salary FROM employees;
```
### 6. Find Employes with a Specific Role (e.g., Manager)
```sql
SELECT * FROM employees WHERE role = 'Manager';
```
### 7. Search for Employes with Names Containing "An" (Case-Insensitive)
```sql
SELECT * FROM employes WHERE name LIKE '%An%' COLLATE NOCASE;
```
### 8. Find Employes Older than 30 and Earning More than $70,000
```sql
SELECT * FROM employes WHERE age > 30 AND salary > 70000;
```
### 9. Change the Salary of an Employe with ID 100
```sql
UPDATE employe SET salary = 10000 WHERE id = 1;
```
### 10. Update the Address for Employes in the 'Sales' Role
```sql
UPDATE employes SET address = 'New Sales Office, Springfield' WHERE role = 'Sales';
```
### 11. Remove an Employe with ID 101
```sql
DELETE FROM employes WHERE id = 1;
```
### 12. Delete All Employes with Age Less than 20
```sql
DELETE FROM employes WHERE age < 20;
```
