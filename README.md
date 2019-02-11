<h1>Springboot Rest Application that demonstrates CRUD operations</h1>
Author: Sohail Nasim <BR />

<h2>How to run it</h2>
1. Make sure you have maven (https://maven.apache.org/download.cgi) installed. Add the bin directory to your PATH.<BR />
2. Install the Git bash (https://git-scm.com/download) or download the repository zip file and unzip it <BR />

Run following commands <BR />
3. <code>cd Springboot-Rest-Example</code> <BR />

4. <code>mvn package</code> <BR />

To run the the boot microservice run following command <BR>

5. <code>java -jar target/UserAdmin-0.0.1-SNAPSHOT.jar</code>

<h2>API documentation for Rest service</h2>
http://localhost:8888/swagger-ui.html <BR />

<h2>Http operations Examples</h2>

1. GET: http://localhost:8888/users <BR />
2. POST: http://localhost:8888/users <BR />
Request <BR />
Content-Type: application/json<BR />
	Body: <BR />
```

{
  "username": "jdoe",
  "password": "password",
  "firstName": "John",
  "lastName": "Doe",
   "emailAddress": "jdoe@youremaildomain.com"
}

```

3. GET: http://localhost:8888/users/jdoe <BR />
	
	Response <BR />
	
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

4. DELETE: http://localhost:8888/users/jdoe <BR />

5. PATCH: http://localhost:8888/users/jdoe <BR />
Request <BR />
Content-Type: application/json<BR />
	Body: <BR />
```

{
  "firstName": "John",
  "lastName": "Doe",
   "emailAddress": "jdoe@youremaildomain.com"
}

```


	

	
	


