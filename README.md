## Student_Registeration_SpringMVC_JDBC

A simple web application to register and view books using Spring MVC, JDBC, and JSP. Built for academic learning and demonstration of MVC architecture, form handling, and database integration.

## Project Structure
Student_Registration_SpringMVC_JDBC/

├── src/

│   ├── main/

│   │   ├── java/

│   │   │   └── com/cdac/

│   │   │       ├── Student.java              # Model class representing a student

│   │   │       ├── StudentController.java    # Handles HTTP requests and maps to views

│   │   │       └── StudentDAO.java           # Data Access Object for database operations

│   │   └── resources/

│   │       ├── applicationContext.xml     # Spring configuration for beans and JDBC
│   │           

│   └── webapp/

│       ├── WEB-INF/

│       │   ├── web.xml                    # Deployment descriptor

|       |   |-- dispatcher-servlet.xml     # Spring MVC dispatcher configuration

│       │   └── views/

│       │       ├── register.jsp           # Form to register a new student

│       │       └── viewbook.jsp           # Displays list of registered student

├── pom.xml                                # Maven build configuration

├── README.md                              # Project overview and setup instructions

## 🚀 Setup Guide
Prerequisites:
Java 8+

Apache Tomcat 9+

Maven

MySQL or MariaDB

## Steps to Run
1. Clone the repository
   git clone https://github.com/akshayuparikar/Student_Registration_SpringMVC_JDBC.git

2.Configure database

Create a database named db
Create a table:
CREATE TABLE student (
  id INT PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(255),
  email VARCHAR(255),
  course VARCHAR(255)
);

3. Update JDBC credentials
Edit applicationContext.xml with your DB username and password.

4. Build the project
mvn clean install

5. Deploy to Tomcat
Copy the WAR file to webapps/ or deploy via Tomcat manager.

6.Access the app
http://localhost:8080/Student_Registration_SpringMVC_JDBC/register

## Features
🧑‍🎓 Student Registration: Add new students with name, email, course.

📄 View Students: Display all registered students from the database.

🔗 Spring MVC Architecture: Clean separation of concerns using Controller, DAO, and Model.

🛠️ JDBC Integration: Direct database access using Spring JDBC templates.

🧩 JSP Views: Simple and responsive UI using JSP pages.

🧪 Maven Build: Easy dependency management and build lifecycle.
