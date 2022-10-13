# MONOLITHIC SERVICES

--------------------------

![Monolithic Services](https://media.geeksforgeeks.org/wp-content/uploads/20200322175817/monolithic.jpg)

* In the word MONOLITHIC, ### Mono means **Single** and ### Lithic means **Store**.
* Monolith means composed all in one piece.
* In this all the fuctionality of application store in a single platform.
* In this a user HTTPs request has directly going to the database,and then database directly response to it.
### Let's take an Example:
		*If a developer makes a Tour&Travles app, that use for booking tours and travel pacakages and for hotels booking.
##### This app consists of mainly four services,
*   i) Tour&Travels bookings
*  ii) Hotel's Bookings
* iii) Payment
* iv) Sign in
* In this app all this services will pe put in a one big app server. and they all are closely couple to each other.
* In this app if you want to make a change on only one thing So, for that you have to change to whole Application.
* If you want to expand your Hotel's Boooking Services,So for that you have to redevelop the whole application.
* At that time , if someone has to check for tours&Travles so he can't. Because of that the whole app is shut.

##### Disadvantages Of Monolithic Services 

- It is rigid in its structure.
- It becomes too large with time and hence,it's difficult to manage.
- It slows down the application starting time. 
- It is not reliable,If there is bug in any one modele\fuction , so that can be drop down your whole application.
- You Have to redevelop your whole application for a single update.
- It lacks to adopt new technology.

##### Advantages Of Monolithic Services 

- It is easy and simple to  develop.
- The deployment becomes simple and easy.
- It is Simple for test,as you can easily test your new updates in the appliction.
- It is not more complex than microservices.