<h2 align = "center"> 1. DataBase </h2>

### 1. Create a Database and Table for Employes

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
VALUES (1, 'Fenish Patel', 'Student', 10000, 18, '123 xyz', '6353600958');
```

### 3. Add Multiple Employees with Selective Data

To add multiple employes with selective data (assuming other fields can be defaulted or null):

```sql
INSERT INTO employes (name, role, salary, age, address, phone) 
VALUES 
VALUES (1, 'Fenish Patel', 'Student', 10000, 18, '123 xyz', '6353600958');
VALUES (2, 'Darshan Patel', 'Student', 10000, 18, '123 xyz', '6353600958');
```

### 4. Retrieve All Employe Information

```sql
SELECT * FROM employes;
```

### 5. Get Specific Columns for All Employes (e.g., name, salary)


```sql
SELECT name, salary FROM employes;
```

### 6. Find Employes with a Specific Role (e.g., Manager)

```sql
SELECT * FROM employes WHERE role = 'Manager';
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
UPDATE employes SET salary = 80000 WHERE id = 100;
```

### 10. Update the Address for Employes in the 'Sales' Role

```sql
UPDATE employes SET address = '456 abc' WHERE role = 'Sales';
```

### 11. Remove an Employee with ID 101

```sql
DELETE FROM employes WHERE id = 1;
```

### 12. Delete All Employes with Age Less than 20

```sql
DELETE FROM employes WHERE age < 5;
```
