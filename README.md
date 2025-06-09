# Microservices App with Spring Cloud

This project is a basic e-commerce system demonstrating microservice architecture using Spring Cloud.

In a microservice architecture, the application is broken into independent, self-contained services, each responsible for a specific piece of functionality. 

In this application :
* __Auth Service__: Manages login/logout, signing in, user authentication.

* __Product Service__: Manages the list of products.

* __Cart Service__: Manages the shopping cart.

* __Frontend Service__: UI for users (runs on port 3000).

* __Gateway Service__: A reverse proxy that routes incoming requests to the correct backend service (via paths like /auth/**, /products/**, etc.).

Each service runs as a separate module and can be started independently, promoting better scalability, maintainability, and separation of concerns.
The Gateway serves as a central entry point, coordinating communication between frontend and backend services.

This setup replicates how large-scale systems are architected in the real world, where business logic is split across multiple isolated services for better flexibility and reliability.

## Sample Users for different Roles
| Role(s)        	 | Username 	        | Password 	  |
|------------------|-------------------|-------------|
| ADMIN          	 | _admin_        	 | _pass_   	 |
| USER          	 | _user_    	       | _pass_   	 |
