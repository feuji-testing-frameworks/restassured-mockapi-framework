### Mock API Testing Using Java-Seleniumn-TestNG

## Description

This project is designed for testing a MockAPI using Selenium WebDriver with the TestNG framework in Java. It allows you to automate API testing, ensuring that your endpoints function correctly.

## Prerequisites

Before you begin, ensure you have the following installed:

- Java JDK 8 or higher
- Maven
- An IDE (Eclipse, IntelliJ IDEA, etc.)

## Project Structure

```plaintext
restassured-mockapi-framework
├── src
│   ├── test
│   │   ├── java
│   │   │   └── com
│   │   │       └── restassured
│   │   │           ├── base
│   │   │           │     └── Base.java
│   │   │           ├── endpoints
│   │   │           │       ├── BookingAPIEndPoint.java
│   │   │           │       └── Routes.java
|   |   |           ├── mockserver    
│   │   │           │       └── MockServer.java
|   |   |           ├── payloads    
│   │   │           │       ├── BookingDates.java
|   |   |           |       ├── BookingDetails.java
│   │   │           │       └── TokenCreation.java
│   │   │           └── test
|   |   |               ├── ApiBookingTest.java
│   │   │               └── MockApiTest.java
│   │   └── resources
│   │       └── log4j2.properties
├── pom.xml
└── testng.xml
```

- **Base.java** : Base class for setting up and tearing down tests.
- **MockServer.java** : MockServer class for setting up and tearing down the mock server.
- **ApiBookingTest.java** : This class contains the API testcases.
- **MockApiTest.java** : This class contains the Mock API testcases.
- **pom.xml** : Maven configuration file.
- **testng.xml** : This file is used for running the testcases.

## Setup Instruction

1. **Clone the Project** : Clone the project repository from GitHub using the following command:

    `https://github.com/feuji-testing-frameworks/restassured-mockapi-framework.git`

2. **Install dependencies** : If you are using IDE it will automatically install dependecies present in pom.xml or if we use command prompt for download the dependencies using the following command

    `mvn clean install`

3. **Running Tests** : For running the tescases using the following command in command prompt or if we use IDE right click on testng.xml file and select Run As then click on TestNG suite

    `mvn test`
