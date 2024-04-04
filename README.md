# ChaTop

An application for managing vacation home reservations, offering users the ability to book accommodation or list their own property for rent.

The Front-end uses :  
![Static Badge](https://img.shields.io/badge/Angular-14.1.3-red)
![Static Badge](https://img.shields.io/badge/Angular_Material-14.1.3-blue)

The Back-end uses :  
![Static Badge](https://img.shields.io/badge/Java-17-orange)
![Static Badge](https://img.shields.io/badge/Maven-4.0.0-purple)
![Static Badge](https://img.shields.io/badge/Spring_Boot-3.1.5-green)
![Static Badge](https://img.shields.io/badge/JJWT-0.11.5-darkblue)
![Static Badge](https://img.shields.io/badge/SpringDoc-2.2.0-green)

> Spring Boot starter dependency :  
> ![Static Badge](https://img.shields.io/badge/Web-grey) > ![Static Badge](https://img.shields.io/badge/Security-grey) > ![Static Badge](https://img.shields.io/badge/DataJPA-grey) > ![Static Badge](https://img.shields.io/badge/Lombok-grey) > ![Static Badge](https://img.shields.io/badge/OAuth2Client-grey) > ![Static Badge](https://img.shields.io/badge/MySQLDriver-grey)

## Getting started

### Clone the project

Clone the project in the directory of your choice :

> git clone https://github.com/CodeByGaetan/ChaTop.git

### Back-end

- Open your IDE (VS Code, Eclipse, etc.) in the directory : `/ChaTop/ChaTopApi`
- Run `mvn spring-boot:run` to launch the back-end in developpment mode
- Or run `mvn package` to build the project and then run `java -jar target/api-0.0.1-SNAPSHOT.jar` to launch the built package.

### Front-end

- Open your IDE (VS Code, Eclipse, etc.) in the directory : `/ChaTop/ChaTopWeb`
- Run `npm install` to install the dependencies
- Run `ng build` to build the project. The build artifacts will be stored in the `/dist/` directory.
- Run `ng serve` to start the front-end development server
- To use the app, navigate to http://localhost:4200/

### Database

MySQL Database install :

- Install mySQL on the localhost and enable the service
- From this app root directory, launch and connect to mySQL
- Run `CREATE DATABASE chatopdb;` to create the database
- Run `USE chatopdb;` to use the newly created database
- Run `SOURCE script_bdd.sql;` to create the database tables
- Run `CREATE USER 'TheUsername'@'%' IDENTIFIED BY 'ThePassword';` to create the MySQL user for the app. The username and password must be the same than in the application.properties file.
- Run `GRANT ALL ON chatopdb.* to 'TheUsername'@'%';` to give ChâTop database access to the new user

## Ressources

### API Documentation

JSON documentation : http://localhost:3001/api/v3/api-docs
HTML documentation : http://localhost:3001/api/swagger-ui/index.html

### Mockoon env

Download Mockoon here: https://mockoon.com/download/

After installing you could load the environement

> /ChaTop/ChaTopWeb/ressources/mockoon/rental-oc.json

directly inside Mockoon

> File > Open environmement

For launching the Mockoon server click on play bouton

Mockoon documentation: https://mockoon.com/docs/latest/about/

### Postman collection

For Postman import the collection

> /ChaTop/ChaTopWeb/ressources/postman/rental.postman_collection.json

by following the documentation:

https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#importing-data-into-postman
