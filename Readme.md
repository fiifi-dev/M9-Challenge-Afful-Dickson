## Module Challenge: Record Store API Secured

### Description
This app uses oauth to authenticate clients app.

Two seperate apps are created:

oauth-server: for authenticating clients
record-store-api: for a client app that uses the the above for authenticating its requests

### Database Description

user: root
password: testpass123
database: auth_server

Feel free to change it to suit your database crendentials

### Note:
I have included the Insomia.json for the testing.

## Entra Dependencies
NB: In order for the record-store-app to run with java 8, I added two extra dependencies:

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

### Runninng Applications
- Check application.properties and set appoporiate msql root and password 
- Run data.sql in DBeaver
- Run oauth-server app first
- Then Run record-store-api

 
