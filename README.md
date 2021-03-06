# CheckMate Web App
<img src="https://github.com/DaniSestan/CheckMate-Web-App/raw/master/checkmate-web.png" alt="Checkmate Web App" title="CheckMate Web App" width="25%" height="25%" />

## Description
This project is currently in development. The application is designed to work alongside a refactored version of the [CheckMate Test Automation Framework](https://github.com/DaniSestan/CheckMate). 

The application provides a simple UI that asks for user input needed to generate the scripts and data sets that will automate tests for web applications. All test-related data would be stored to a database. Whenever the user wants to run tests, they would start the framework, which runs as a desktop application. The framework would establish a connection to the database, allowing it access to the scripts and data sets needed to execute tests. **No coding or scripting of any kind is required to create and execute tests.**

Test sets, data sets, and reporting generated by the framework are stored and accessible to users through the application. With persistent storage, users' data can be stored to an account, allowing them to access modify run their data for future test runs. This includes run configurations for test sets, individual scripts, test data, as well as reports, screenshots and  custom keywords, reports, and screenshots. The UI will allow users to easily search for and filter through this data. The app also provides access control: permissions can be set that grant certain users with access to stored data. 

The framework itself will be modified to run through the fiel
## Built With:
This project is designed as full-stack application, built with the following tools.
* **Java Development Kit 8** : provides the libraries, JVM, and other components to run the app, along with tools for compiling and debugging
* **Selenium** : playback tool for authoring functional tests without the need to learn a test scripting language.
* **Spring** : Java based framework used for the backend REST API
    * **Spring Boot 2**
    * **Spring Web** 
    * **Spring Data**
    * **Spring Initializer**
* **Gradle** : Dependency management
* **MongoDB** : Document database – used by the back-end application to store its data as JSON (JavaScript Object Notation) documents
* **Express** : Back-end web application framework running on top of Node.js
* **React** : Front-end web app framework; runs the JavaScript code in the user's browser, allowing the application UI to be dynamic
* **Node.js** : JavaScript runtime environment – allows the application back-end to be implemented in JavaScript
* **AWS** : The application will be deployed on an Ubuntu AWS EC2 instance.


## Features:
* **No scripting/coding required:** scripts and data sets are generated for by the web app. The UI will prompt the user for input used in executing test steps. Scripts and data sets are then downloaded and the framework, run on as a separate desktop application, will be able to access a local copy of these files to execute the tests.
* **Storage:** All test-related data will be stored and accessible online to anyone with an account. Teams can share data amongst members, and allow/restrict access to view and/or modify files.
* **Easy navigation:** users would easily be able to search and filter through the data they need.
* **Reusability:** the framework is set apart by its ability to implement and maximize reusability. Scripts can be modified and allowed to run from any point in the test. This is particularly useful when troubleshooting failpoints. This is done by preserving the session data from the browser while running each test. The driver can then step "back in time", essentially starting from any point in a prior test instance, using the recorded session data. Tests are also modularized, allowing for scripts to be broken down into components which can reused in other test scripts where they are referenced.
* **Keyword-Driven Testing:** with keywords, no coding is required to write test scripts. Testers can add and customize keywords that symbolize the functionalities used in testing.
* **Data-Driven Testing:** allows users to easily create and manipulate large data sets and to test large volumes of data quickly.
* **Reporting:** the framework automatically generates reports and screenshots of the tests, and prints the results to an html file in an easy-to-read format. Reports provide details about each test step, including specifics about where, when, and how the step was executed and what test data was used.
* **Cross Browser/Platform:** Compatible with Windows and Linux and supports all major browsers.
* **Environments:** Build your tests once and run them against multiple environments or using different sets of test data.
