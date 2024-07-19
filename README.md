# Registration Form Project

## Description

This is a Java Swing application for user registration, integrated with a MySQL database to store user details. The application allows users to input their information, which is then displayed on the right side of the form in a structured manner. It includes fields for user ID, name, gender, address, and contact details.

## Features

- **User Registration Form**: Collects user details including ID, name, gender, address, and contact information.
- **Database Integration**: Stores user information in a MySQL database.
- **Data Display**: Shows entered data on the right side of the form in a tabular format.

## Requirements

- **Java Development Kit (JDK)**: Version 8 or above.
- **NetBeans IDE**: For running and editing the Java code.
- **XAMPP**: For managing the MySQL database.

## Setup Instructions

1. **Set Up the Database**

   - Open XAMPP and start the MySQL server.
   - Access phpMyAdmin from [http://localhost/phpmyadmin](http://localhost/phpmyadmin).
   - Create a new database named `Registration`.
   - Execute the following SQL script to create the table:

     ```sql
     CREATE TABLE `registration 2` (
         id INT AUTO_INCREMENT PRIMARY KEY,
         `user id` VARCHAR(255),
         name VARCHAR(255),
         gender VARCHAR(50),
         address VARCHAR(255),
         contact VARCHAR(255)
     );
     ```

2. **Configure Database Connection**

   - Open `Registration.java` in NetBeans.
   - Update the database connection settings in the code to match your local MySQL setup:

     ```java
     private static final String DB_URL = "jdbc:mysql://localhost/Registration";
     private static final String USER = "root";
     private static final String PASS = "";
     ```

3. **Run the Application**

   - Compile and run `Registration.java` in NetBeans.
   - The application will display a registration form where users can enter their information.
