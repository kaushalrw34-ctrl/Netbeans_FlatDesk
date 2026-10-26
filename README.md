# FlatDesk — NetBeans + MySQL version

## Stack
- Apache NetBeans 31
- Java 17+
- Maven WAR
- Tomcat 10.1+
- MySQL 8/9 + MySQL Workbench
- Jakarta Servlets
- JDBC
- JSP/HTML/CSS/JavaScript
- REST APIs using JSON

## 1. Database
Open MySQL Workbench and run `database.sql`.

## 2. MySQL password
Open:
`src/main/java/com/flatdesk/config/DB.java`
and replace:
`YOUR_MYSQL_PASSWORD`

## 3. NetBeans
File > Open Project and select this folder. Let Maven download dependencies.
Add Tomcat 10.1 as the server. Run the project.

## 4. URLs
Home: `/FlatDesk/`
Login: `/FlatDesk/login.jsp`
Admin: `/FlatDesk/admin.jsp`
Broker: `/FlatDesk/broker.jsp`
User: `/FlatDesk/user.jsp`

## 5. REST APIs
GET  `/api/auth`
POST `/api/auth/login`
GET  `/api/properties`
POST `/api/properties`
DELETE `/api/properties?id=1`
GET  `/api/dashboard`

## Important
The current uploaded FlatDesk HTML is a browser prototype using SQL.js/localStorage. This project changes that architecture to Java/JDBC/MySQL so submitted property data is stored in MySQL.
