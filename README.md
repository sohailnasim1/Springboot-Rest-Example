# Springboot Restful web services CRUD example
Contributer: **Sohail Nasim**

This project was developed in [Spring Tool Suite](http://spring.io/tools/sts)

## Database

**H2  Embedded (Local) file based Database**

Schema and 'USERS' table is generated when Springboot application starts

URL: (http://localhost:8888/h2)

DB Name: useradmindb

Username: sa

Password:


## How to run it
1. You need JDK 1.8 to run this project.
2. Make sure you have [Apache Maven](https://maven.apache.org/download.cgi) installed. Add the bin directory to your PATH.
3. Install the [Git Bash](https://git-scm.com/download) or download the repository zip file and unzip it.

Run following command to compile and to create the jar file:

```
cd Springboot-Rest-Example
mvn package

```

How to run Springboot microservices locally:

```
java -jar target/UserAdmin-0.0.1-SNAPSHOT.jar
```

## API documentation for Rest service
http://localhost:8888/swagger-ui.html

## Examples

* GET: http://localhost:8888/users


* POST: http://localhost:8888/users


**Request:**

Content-Type: application/json

Body:

```
{
  "username": "jdoe",
  "password": "password",
  "firstName": "John",
  "lastName": "Doe",
   "emailAddress": "jdoe@youremaildomain.com"
}
```

* GET: http://localhost:8888/users/jdoe
	
**Response:**
	
```
{
    "username": "jdoe",
    "password": "password",
    "firstName": "John",
    "lastName": "Doe",
    "emailAddress": "jdoe@youremaildomain.com",
    "active": "Y"
}
```

* DELETE: http://localhost:8888/users/jdoe


* PATCH: http://localhost:8888/users/jdoe

**Request:**

Content-Type: application/json

Body:

```
{
  "firstName": "John",
  "lastName": "Doe",
   "emailAddress": "jdoe@youremaildomain.com"
}

```