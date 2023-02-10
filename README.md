# example

# Gender API app
> ### This guide walks you through the process of installing a Spring application connected to a MySQL Database(as opposed to an in-memory, embedded database, which most of the other guides and many sample applications use). It uses Spring Data JPA to access the database, but this is only one of many possible choices.

## Table of Contents
* [Requirements](#Requirements)
* [Create the Database](#Create-the-Database)
* [Technologies and Frameworks Used](#technologies-and-frameworks-used)

## Requirements
1. Java - 1.8.x

2. Maven - 3.x.x

3. MySQL - 5.x.x

## Create the Database
Open a terminal (command prompt in Microsoft Windows) and open a MySQL client as a user
who can create new users.

For example, on a Linux system, use the following command;

====
[source, sh]
----
$ sudo mysql --password
----
====

NOTE: This connects to MySQL as `root` and allows access to the user from all hosts. This
is *not the recommended way* for a production server.

To create a new database, run the following commands at the `mysql` prompt:

====
[source, mysql]
----
mysql> create database db_example; -- Creates the new database
mysql> create user 'springuser'@'%' identified by 'ThePassword'; -- Creates the user
mysql> grant all on db_example.* to 'springuser'@'%'; -- Gives all privileges to the new user on the newly created database
----
====


## Technologies and Frameworks Used
- Spring Boot 3.0.1 [_spring-boot_](https://spring.io/projects/spring-boot)
- Spring Data JPA
- Spring Web MVC
- Flyway migration
- ModelMapper
- Database - H2 (in memory)
- Docker [_docker_](https://www.docker.com/)
- IDE - IntelliJ IDEA [_intellij-idea_](https://www.jetbrains.com/)
