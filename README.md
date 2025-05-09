# 📝 Assignment: Database Design and Normalization

## 🎯 **Learning Objectives**
* 🛠️ **Understand the principles of good database design** and **normalization**.
* 💡 **Apply normalization techniques** to improve database structure and efficiency.
* 🔍 **Learn First, Second, and Third Normal Forms** (1NF, 2NF, 3NF) to eliminate redundancy and optimize data storage.

---

## 📋 **What You'll Need**
* 💻 A computer with internet access.
* ✍️ A code editor (e.g., Visual Studio Code).
* 🖥️ MySQL Workbench or another SQL database environment.

---


## 📝 Submission Instructions  
📂 Write all your SQL queries in the **answers.sql** file.  
✍️ Answer each question concisely and make sure your queries are clear and correct.  
🗣️ Structure your responses clearly, and use comments if necessary to explain your approach.

--- 

## 📚 Assignment Questions

---

### Question 1 Achieving 1NF (First Normal Form) 🛠️
Task:
- You are given the following table **ProductDetail**:

| OrderID | CustomerName  | Products                        |
|---------|---------------|---------------------------------|
| 101     | John Doe      | Laptop, Mouse                   |
| 102     | Jane Smith    | Tablet, Keyboard, Mouse         |
| 103     | Emily Clark   | Phone                           |


- In the table above, the **Products column** contains multiple values, which violates **1NF**.
- **Write an SQL query** to transform this table into **1NF**, ensuring that each row represents a single product for an order

SELECT
    OrderID,
    CustomerName,nancy
    TRIM(product) AS Product
FROM daisy
    ProductDetail,
    unnest(string_to_array(Products, ',')) AS product
ORDER BY
    OrderID, Product;
john
--- 

### Question 2 Achieving 2NF (Second Normal Form) 🧩

- -- Create Customers table
CREATE TABLE Customers (
    OrderID INT PRIMARY KEY,
    CustomerName VARCHAR(100)
);

-- Create Products table
CREATE TABLE Products (
    Product VARCHAR(100) PRIMARY KEY,
    Quantity INT
);

-- Create OrderDetails table
CREATE TABLE OrderDetails (
    OrderID INT,
    Product VARCHAR(100),
    PRIMARY KEY (OrderID, Product),
    FOREIGN KEY (OrderID) REFERENCES Customers(Order-- Create Customers table
CREATE TABLE Customers (
    OrderID INT PRIMARY KEY,
    CustomerName VARCHAR(100)
);

-- Create Products table
CREATE TABLE Products (
    Product VARCHAR(100) PRIMARY KEY,
    Quantity INT
);

-- Create OrderDetails table
CREATE TABLE OrderDetails (
    OrderID INT,
    Product VARCHAR(100),
    PRIMARY KEY (OrderID, Product),
    FOREIGN KEY (OrderID) REFERENCES Customers(+22378934562),
    FOREIGN KEY (Product) REFERENCES Products(nail)
);
ID),
    FOREIGN KEY (Product) REFERENCES Products(nail)
);




---
Good luck 🚀
