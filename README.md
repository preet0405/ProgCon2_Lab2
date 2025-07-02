📘 README - JavaFX CRUD MySQL Application
👤 Student Information
Name: Preet Patel

Student ID: 123456

Date: July 2, 2025

📌 Project Title
JavaFX Customer Management Application (CRUD + MySQL)

I have taekn help form my peers Piyush and Ved as well as used Chatgpt for the jdbc setup and learning some new functions from it.

🧾 Project Description
This JavaFX application allows users to manage customer data stored in a MySQL database. The interface provides full CRUD functionality:

Create (Insert)

Read (View)

Update

Delete

It connects to a local MySQL database and uses JDBC for data operations. The data is displayed in a TableView, and interaction is handled via JavaFX controls.

🖥️ Technologies Used
Java 17+

JavaFX SDK 21 or 24

MySQL Server

MySQL Connector/J (JDBC Driver)

Command Prompt

GitHub (for version control and hosting)

📂 Project Structure
arduino
Copy
Edit
JavaFX_CRUD_MySQL.java             ← Main application file
mysql-connector-j-8.4.0.jar        ← JDBC driver
run-javafx-app.bat                 ← Script to compile and run
README.md                          ← Project documentation
🖼️ GUI Layout
The GUI includes:

A TableView showing all customers

Input fields: ID, Name, Email

Buttons: Insert, Update, Delete, View Data

📸 Screenshot should be inserted here with Name, ID, and Date visible

🗃️ Database Structure
Database: testdb
Table: customers

sql
Copy
Edit
CREATE DATABASE testdb;

USE testdb;

CREATE TABLE customers (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100)
);
📸 Include screenshot of the table with sample data in phpMyAdmin or MySQL Workbench

⚙️ How to Run
✅ Prerequisites
JavaFX SDK (e.g., C:\javafx-sdk-24.0.1)

MySQL Server installed and running

MySQL JDBC .jar downloaded

🔄 Compile and Run (Command Prompt)
bash
Copy
Edit
javac --module-path "C:\javafx-sdk-24.0.1\lib" --add-modules javafx.controls,javafx.fxml -cp .;mysql-connector-j-8.4.0.jar JavaFX_CRUD_MySQL.java

java --module-path "C:\javafx-sdk-24.0.1\lib" --add-modules javafx.controls,javafx.fxml -cp .;mysql-connector-j-8.4.0.jar JavaFX_CRUD_MySQL
