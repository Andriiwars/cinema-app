## Description
This is simple web-application 
that supports authentication, registration 
and CRUD operations with different entities. 
You can check movie sessions, cinema halls, 
buy tickets, add new movies, add order to shopping cart etc.

## Features
This project has multiple endpoints with user and admin access.

- POST: /register - all
- GET: /cinema-halls - user/admin
- POST: /cinema-halls - admin
- GET: /movies - user/admin
- POST: /movies - admin
- GET: /movie-sessions/available - user/admin
- POST: /movie-sessions - admin
- PUT: /movie-sessions/{id} - admin
- DELETE: /movie-sessions/{id} - admin
- GET: /orders - user
- POST: /orders/complete - user
- PUT: /shopping-carts/movie-sessions - user
- GET: /shopping-carts/by-user - user
- GET: /users/by-email - admin

## Technologies
- Java version 11 
- Spring  
- Hibernate 
- Apache Tomcat (v9.0.50)
- MySQL 
- Maven

## How to run project
- Install MySQL and Apache Tomcat 9.0.50
- Install and configure and create a schema in MySQL
- Clone this project
- Configure db.properties file from main.resources directory to create connection to db:
```java
    db.driver=com.mysql.cj.jdbc.Driver
    db.url=URL
    db.user=LOGIN
    db.password=PASSWORD
```
- Add Tomcat configuration to your project. Use `/` as your Tomcat application context

After that you will be able to log in as a user or administrator :

`USER`:
```java
username - User@gmail.com
password - 321321
```
`ADMIN`:
```java
username - Admin@gmail.com
password - 123123
```