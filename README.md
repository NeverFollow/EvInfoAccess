EvInfoAccess
============

Project: 	   EvInfoAccess		  

https://www.hackerleague.org/hackathons/zero-emission-innevation/hacks/evinfoaccess

• Category:  	Travel Planning, Car Sharing, Improve Range Confidence

• APIs&amp;Tools: 	Esri, LeafSpy, OSIsoft, Twilio  

• Repository: 	https://github.com/NeverFollow/EvZigZag  

Problem  

While a lot of mobile applications have been developed specifically to facilitate the usage of electric vehicles (EVs), such as improving range confidence, most of those applications will not be fully usable when renting an EV because the user is not the owner of the vehicle. 

So a driver will need to enter manually the car battery status information to the application used during a trip for finding and selecting a charging station. Entering battery status information will not be very practical for most of the drivers and will not be very precise. 

Solution 

The proposed solution is to implement a service providing a secure interface allowing applications, used by a driver renting an EV, to access the diagnostic information provided by the car manufacturer to the registered rental car. 

Future extensions for this project will be to allow a driver of a rental EV to install personal applications, using Bluetooth or NFC, to the car’s display during the lease of the car. 

How “EvInfoAccess” works 

This project will be articulated around two main projects. The first project will be a mobile client app, (EvInfoAccess Client), running on various types of smartphones, or running directly on the EV’s internal display. 

The mobile client app will be used first to enter information about the rented car. This will be used to access the registered rental car diagnostic information. Second, the client app would be used to select which application will be authorized for accessing the service and what type of information should be accessible. 

The mobile client app should be able to interact with various applications used by the driver during the trip to inform those applications about itinerary changes or up-to-date battery diagnostic information. 

The second part of the project will be a server broker (EvInfoAccess Server), allowing the mobile app to securely get access to the diagnostic information regarding the battery status. 

Initially a car rental company will register the EVs for which diagnostic battery information will be made available, using the secure broker. Then, every time an EV get rented, the car rental company will make available to the server broker, information regarding driver’s credentials and the duration of the lease. 

Then, when a new user will be driving an rental EV, the user’s mobile client app will make requests for receiving up-to-date battery’s diagnostic information from the secure broker. The battery information will be then propagated to the user’s applications used for locating a charging station and making reservation arrangements.
