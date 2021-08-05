# sql_query

[Try](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_columns)

```sql
SELECT * FROM Customers;
SELECT CustomerName, City FROM Customers;
SELECT CustomerName FROM Customers;
```

```sql
SELECT DISTINCT Country FROM Customers;
SELECT COUNT(DISTINCT Country) FROM Customers;
```

```sql
SELECT * FROM Customers WHERE Country='Mexico';
SELECT * FROM Customers WHERE City IN ('Paris','London');
SELECT * FROM Customers WHERE City LIKE 's%';
SELECT * FROM Products WHERE Price BETWEEN 50 AND 60;
SELECT * FROM Products WHERE Price <> 18; //SQL this operator may be written as !=
SELECT * FROM Products WHERE Price <= 30;
SELECT * FROM Products WHERE Price >= 30;
SELECT * FROM Products WHERE Price < 30;
SELECT * FROM Products WHERE Price > 30;
SELECT * FROM Products WHERE Price = 18;
```

```sql
SELECT * FROM Customers WHERE Country='Germany' AND (City='Berlin' OR City='München');
SELECT * FROM Customers WHERE NOT Country='Germany' AND NOT Country='USA';
```

```sql
SELECT * FROM Customers ORDER BY Country;
```

```sql
INSERT INTO Customers (CustomerName, ContactName, Address, City, PostalCode, Country)
VALUES ('Cardinal', 'Tom B. Erichsen', 'Skagen 21', 'Stavanger', '4006', 'Norway');
```

```sql
SELECT CustomerName, ContactName, Address FROM Customers WHERE Address IS NULL;
SELECT CustomerName, ContactName, Address FROM Customers WHERE Address IS NOT NULL;
```

```sql
UPDATE Customers SET ContactName = 'Alfred Schmidt', City= 'Frankfurt' WHERE CustomerID = 1;
```

```sql
DELETE FROM Customers WHERE CustomerName='Alfreds Futterkiste';
```

```sql
SELECT * FROM Customers LIMIT 3;
SELECT * FROM Customers WHERE Country='Germany' LIMIT 3;
```

```sql
SELECT MIN(Price) AS SmallestPrice FROM Products;
SELECT MAX(Price) AS LargestPrice FROM Products;
```

```sql
SELECT COUNT(ProductID) FROM Products;
SELECT AVG(Price) FROM Products;
SELECT SUM(Quantity) FROM OrderDetails;
```

```sql
SELECT * FROM Customers WHERE CustomerName LIKE 'a%';       --Finds any values that start with "a"
SELECT * FROM Customers WHERE CustomerName LIKE '%a';       --Finds any values that end with "a"
SELECT * FROM Customers WHERE CustomerName LIKE '%or%';     --Finds any values that have "or" in any position
SELECT * FROM Customers WHERE CustomerName LIKE '_r%';      --Finds any values that have "r" in the second position
                                                                --Around the Horn
                                                                --Drachenblut Delikatessend
SELECT * FROM Customers WHERE CustomerName LIKE 'a_%';      --Finds any values that start with "a" and are at least 2 characters in length
                                                                --Alfreds Futterkiste
                                                                --Ana Trujillo Emparedados y helados
SELECT * FROM Customers WHERE CustomerName LIKE 'a__%';     --Finds any values that start with "a" and are at least 3 characters in length
SELECT * FROM Customers WHERE CustomerName LIKE 'a%e';      --Finds any values that start with "a" and ends with "e"
                                                                --Alfreds Futterkiste
SELECT * FROM Customers WHERE City LIKE '_ondon';           --Selects all customers with a City starting with any character, followed by "ondon":
                                                            --London	
SELECT * FROM Customers WHERE City LIKE 'L_n_on';
SELECT * FROM Customers WHERE City LIKE '[bsp]%';           --Selects all customers with a City starting with "b", "s", or "p"
                                                            --Paris 
                                                            --São Paulo 
                                                            --Portland 
                                                            --Seattle 
                                                            --Buenos Aires
SELECT * FROM Customers WHERE City LIKE '[a-d]%';           --A B C D
SELECT * FROM Customers WHERE City LIKE '[!bsp]%';
SELECT * FROM Customers WHERE City NOT LIKE '[bsp]%';
```

```sql
```

```sql
```

```sql
```

```sql
```

```sql
```

---

```
Copyright 2021 M. Fadli Zein
```