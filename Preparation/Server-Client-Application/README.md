# **Preparation Project**
# **Weather JAVA EE + Angular+  UI**
**Project name:** Weather JAVA EE + Angular8+
**Tech stack:** J2EE, Angular8+
## **Lesson goals**
The purpose of this lesson is to familiarize students with the following frameworks and technologies:

**Java EE 6+**
1. Java EE Project structure
1. Rest WebServices (JAX-RS)
1. Dependency Injection (DI)
1. Java Persistence API (JPA)
1. Background servies (Scedulers)
1. Access external services via Rest API (Rest Client)
1. Authentication
1. Session management

**Angular 8+**
1. Basic project structure
1. Components
1. Page layout
1. Service providers

## **Homework description**
Create a client-server application, the main function is to show a cities weather (temperature) data on a simple web interface, so we call our application "WeatherApp"

### **The main functions of the WeatherApp**
1. Enter a city name, and fint the weather information from a public, external API (eg. openweathermap.com)
1. Save the weather information to local database for the city that was entered
1. List the cities and weather information that are in our local database
1. Can delete city from out local database
1. Weather data is automatically refreshed in the background using a scheduled service

### **Use cases**
1. Add new city weather data
1. Get list of weaher data from our local database
1. Delete city from out local database

### **Tasks to be completed**
#### **Backend**
1. Create and configure the JavaEE project, called WeatherApp
1. Configure database 
   0. Create schema: weatherapp
   0. Create table: weatherdata 
      0. cityname - name of the city
      0. temperature - the last known temperature of the city
      0. time - the time of the measurement
1. Confure application server.
1. Create services and Rest interfaces.
1. Build and deploy application.
1. Test application's Rest API

#### **Frontend**
1. Create Angular 4 project
1. Create a user interface components as shown below in the diagram
   0. app.component
   0. search.component
   0. citylist.component
   0. cityitem.component
1. Connect server side calls
1. Build + Run + Test the application


## **Checklist**

|**Component**|**Task**|**Description**|**Accepted (Y/N)**|
| :-: | :-: | :-: | :-: |
|Backend|Create project structure|Create a new Java EE application project in your favorite IDE and configure it.|--|
|Backend|Build and deploy project|Build and run the empty project on a J2EE container server.|--|
|Database|Create database schema and tables|Create the necesary database schema and the tables.|--|
|Backend|Create entity class and basic JPA functions|Create model for watherdata and save it, load it from database successfully.|--|
|Backend|Hello world Rest API|Create a simple REST API which returns only "Hello Weather"|--|
|Backend|Rest API: addCity|Implement and test the addCity API. Save data to database.|--|
|Backend|Rest API: listCities|Implement and test listCities API. Have to load data from local DB.|--|
|Backend|Rest API: deleteCity|Implement and test deleteCity API. Have to delete data from local DB.|--|
|Backend|openweathermap API client|Implement a client that calls openweatherapi.org weather REST API by city name. The result must be saved to our local database.|--|
|Backend|Scheduled update service|Implement a the update service which update the cities data from the openweather api.|--|
|Backend|Dependency Injection|Use DI to use Java EE components: update service (EJB), entityManager (JPA) etc...|--|
|Backend|Error handling|Handle errors in the Rest API with general way.|--|
|Backend|Logging|Log the events what happens in the REST API.|--|
|Frontend|Create project structure|Create a new empty Angular project with Hello Weather message only.|--|
|Frontend|Build and deploy project|Build and run the empty project on a webserver.|--|
|Frontend|Component: Add city component|Create the visuals of the Add city component, without REST calls.|--|
|Frontend|Component: List cities component|Create the visuals of the List cities component, without REST calls.|--|
|Frontend|Component: City listitem component|Create the visuals of the City listitem component.|--|
|Frontend|Main application component|Layout the other component into the main app screen.|--|
|Frontend|REST: addCity integration|Add server side integration to the Add city component (addCity API call)|--|
|Frontend|REST: listCity integration|Add server side integration to the List cities component (listCities API call)|--|
|Frontend|REST: deleteCity integration|Add server side integration to the City listitem component (deleteCity API call)|--|
|Frontend|Error handling|Handle and visualize possible error messages from the server.|--|
|<p>Backend +</p><p>Frontend</p>|CHECK ALL THE APPLICATION IS WORKING?|CHECK ALL THE APPLICATION IS WORKING?|--|



