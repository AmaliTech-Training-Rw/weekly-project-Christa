## MUSIC LIBRARY MANAGEMENT SYSTEM

### What to change before running the application:
After you have cloned the application, head to application.properties file and change the following lines to appropriate values:

## DATABASE
spring.datasource.username=
spring.datasource.password=
spring.datasource.url=jdbc:postgresql://localhost:5432/mlms?useSSL=false

Note: Here the database name is mlms, if you create another database fill it’s name in the datasource url.

After this you can now run the application.

2. Using the application:
Head to http://localhost:8000/swagger-ui.html to access the Swagger Documentation of the Application.
3. Authentication:
- Creation of An Account

### User Login
Head over to Authentication-Controller and use the endpoint below, It will return a JWT Token. This token is used to access all other endpoints in the application:

After getting the token. Head over to the top of the swagger documentation,
 there is a button called Authorize, Click it and paste the token there.

Note: Before pasting the token, add the Bearer keyword before it.

##### Forexample: - Token:
- String to paste:
yuahjahfb73haja
Bearer yuahjahfb73haja