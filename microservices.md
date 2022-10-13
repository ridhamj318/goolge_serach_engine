# Microservices

-----

![Microservices](https://media.geeksforgeeks.org/wp-content/uploads/20200322182733/microservices.jpg)

* It is an architectural development style in which the application is made up of smaller 
 services that handle a small portion of the functionality.
* Unlike Monolith , Microservices has it's own database.
* So because of that they are independent, and they don't dependent on others.
* In this every services has its own APIs. 
* It is loosely couple to each other. 
* When a user ask for its https file, then the request has passed through the API Gateway, and then it passes to particular services database and then it respond.
* Let's take an example; 
				Suppose a developer makes a Tour&Travles app, that use for booking tours and travel pacakages and for hotels booking.
This app consists of mainly four services,
   i) Tour&Travels bookings
  ii) Hotel's Bookings
 iii) Payment
  iv) Sign in
 So in a microsevices all the servivces has their own database and they are loosely couple to each others and they have their own datbase.
 If you want to expand your Hotel's Boooking Services,So you can do it easily  you don't have to redeploy your whole app , you can work on it and your other services were working 
 effectively.
 So, at that time if anybody has to saw the tours and travels , so he can saw it properly.  

### Advantages of Microservices

- It is easy to manage.
- The deployment of services becomes easy and relaible.
- Large complex application can easily develop.
- If there’s any update in one of the microservices, then we need to redeploy only that microservice.
- Their start and redeploy time are realtive less.
- If a particular microservice is facing a large load because of the users using that functionality in excess, then we need to scale out that microservice only.
- Each microservice can use different technology based on the business requirements.
- If a particular microservice goes down due to some bug, then it doesn’t affect other microservices and the whole system remains intact and continues providing 
  other functionalities to the users.

### Disadvantages Of Microservices.

- Because of distributed system it is much more complex than monolith system. and when the services increases it's complexityu increases.
- In this the developers must have to manage their inter-commucation.
- Independent deployment of microservices is complicated.
- Find a bug is quit difficult in microservices.
- It is costly as compared to Monolithic Services.
- Testing is more difficult as compared to Monolith applications.
- Microservices are less secure as compared to monolithic system , because of inter-commucation ofservices.
