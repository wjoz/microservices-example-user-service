# microservices-example-user-service
The project implements the User Service micro service from the microservices architecture example.

# Details

This project provides a sample User micro service.

Before running this micro service, make sure, you've run the microservices-example-service-discovery project which is the service registry process.

The User Service will register there in order to be able to communicate with the Message Service (microservices-example-message-service). 

# How to Build and Run

1. Make sure to run the Service Discovery micro service the (microservices-example-service-discovery project) that will run on port 1111.
1. Open up a terminal and use the following command: **mvn spring-boot:run** 
2. The User Service will run on port 2222, as specified in application.yml
3. To test, visit [http://localhost:2222/users](http://localhost:2222/users])
4. You can see whether the User Service has registered in the service registry by visiting [http://localhost:1111](http://localhost:1111)