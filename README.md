# chat_api
> #### This guide walks you through the process of installing a Spring application connected to a MySQL Databas. It uses Spring Data JPA to access the database.

## Table of Contents
* [Requirements](#Requirements)
* [Steps to setup](#Steps-to-setup)
* [Technologies and Frameworks Used](#technologies-and-frameworks-used)

## Requirements
1. Java - 17.x

2. Maven - 3.x.x

3. MySQL - 5.x.x

## Steps to setup
**1. Clone the application**

```bash
git clone https://github.com/callicoder/chat_api.git
```

**2. Create Mysql database**
```bash
create database chat_api
```

**3. Change mysql username and password as per your installation**

+ open `src/main/resources/application.properties`

+ change `spring.datasource.username` and `spring.datasource.password` as per your mysql installation

**4. Build and run the app using maven**

```bash
cd chat_api
mvn package
java -jar target/flyway-demo-0.0.1-SNAPSHOT.jar
```

You can also run the app without packaging it using -

```bash
mvn spring-boot:run
```

## Technologies and Frameworks Used
- Spring Boot 3.0.1 [_spring-boot_](https://spring.io/projects/spring-boot)
- Spring Data JPA
- Spring Web MVC
- Flyway migration
- Database - MySQL
- IDE - IntelliJ IDEA [_intellij-idea_](https://www.jetbrains.com/)

## 
The following guides may also be helpful:

1. Learn how to integrate Flyway in your Spring Boot application - https://www.callicoder.com/spring-boot-flyway-database-migration-example/

