# Work Scheduler

## Project Description

The Work Scheduler is a full-stack web application for managing and viewing the shift schedule of a restaurant or retail store. Employees can view the current and upcoming work schedule, and submit time-off requests. Manager-level users can additionally create schedules by assigning employees to shifts on specific days, and can approve time-off requests.

This project is divided into three submodules:

* WorkSchedulerServer
  * A Maven project for the backend server
* WorkSchedulerFrontend
  * An Angular project for the frontend web app
* WorkSchedulerFrontendTest
  * A Maven project that uses selenium and cucumber to test the frontend web app

## Technologies Used

* Java 8
* Spring Boot 2.5.6
    * Spring Data JPA
    * Spring Security
    * Spring Test
    * Spring Web
* JUnit 5
* PostgreSQL 12
* Angular 12
* Selenium 3.8.1
* Cucumber 7

## Features

Implemented Features
* Login, Authorization, Role-based Permissions
* Users can view current and upcoming schedules
* Managers can create schedules and assign employees to shifts
* Users can request time off and view their time off requests
* Managers can approve time off requests

To-do list:
* Secure app with HTTPS
* Add ability for users to set or request recurring unavailabilities
* Set up continuous integration

## Getting Started
1. Clone the repository
```
git clone https://github.com/Commoble/WorkScheduler.git
```
2. Add WorkSchedulerServer/src/main/resources/application.properties files with database connection parameters

```properties
spring.datasource.driver-class-name=org.postgresql.Driver
spring.datasource.url=YOUR_DATABASE_URL
spring.datasource.username=YOUR_DATABASE_USERNAME
spring.datasource.password=YOUR_DATABASE_PASSWORD
spring.jpa.hibernate.ddl-auto=validate
```

3. Add WorkSchedulerFrontendTests/src/test/resources/workschedulerfrontendtests.properties file with selenium parameters

```properties
# path to your selenium driver
driverpath=C:/Program Files/Selenium/geckodriver.exe

# what type of driver it is, allowed values are currently FIREFOX and CHROME
drivertype=FIREFOX
```

## Usage

* Built artifacts are not currently provided.
* Running the WorkSchedulerServer's com.revature.workscheduler.WorkSchedulerApplication#main method will start the backend server.
* The frontend web app can be served by running `ng serve` from the WorkSchedulerFrontend directory.

## Contributors
* Ahmed Sahli
* Keven Mitchell
* Jada Forde
* Joseph Bettendorff
* Victor Gee