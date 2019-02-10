<h1>Springboot Rest Application that demonstrates CRUD operations</h1>
Author: Sohail Nasim <BR />

<h2>API documentation for Rest service</h2>
http://localhost:8888/swagger-ui.html <BR />

<h2>Http operations Examples</h2>

1. GET: http://localhost:8888/users <BR />
2. POST: http://localhost:8888/users <BR />
Request <BR />
	Body: application/json<BR />
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
	
	


