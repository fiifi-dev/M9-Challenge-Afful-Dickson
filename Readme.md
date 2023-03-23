# Module Challenge: Record Store API Secured

This project includes two separate applications that work together to provide a secure and efficient way to authenticate clients and manage their data. The oauth-server is responsible for authenticating client applications, while the record-store-api serves as a client app that uses the OAuth server for authentication purposes.

## Overview
**oauth-server**: This application is responsible for providing secure OAuth authentication for clients. It ensures that only authorized clients can access the protected resources of the record-store-api.
**record-store-api**: This application serves as a client that utilizes the oauth-server for authentication. It is a fully functional API that allows clients to manage and access their record store data.

## Database Description

- user: root
- password: testpass123
- database: auth_server

Feel free to change it to suit your database crendentials

### Note:
I have included the `Insomia.json` for the testing.



### Getting Startted
- Check application.properties and set appoporiate msql root and password 
- Run data.sql in DBeaver
- Run oauth-server app first
- Then Run record-store-api
- import insomia.json into insomia and test endpoints



 ## Entra Dependencies
NB: In order for the `record-store-app` to run with java 8, I added two extra dependencies:

```
<dependency>
	<groupId>com.sun.xml.bind</groupId>
	<artifactId>jaxb-impl</artifactId>
	<version>2.3.1</version>
</dependency>
<dependency>
	<groupId>com.sun.xml.messaging.saaj</groupId>
	<artifactId>saaj-impl</artifactId>
	<version>1.5.1</version>
</dependency>
```
