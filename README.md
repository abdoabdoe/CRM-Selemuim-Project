Automated Testing and Data Handling Documentation
Introduction
The provided Java code represents a testing framework for a web application using Selenium and TestNG. It includes functionality for handling Excel sheets using Apache POI, capturing screenshots, and performing automated login tests on the FreeCRM web application.

1. Class: fileSheet
Purpose
The fileSheet class is responsible for reading data from an Excel file and storing it in a 2D array.

Methods
main(String[] args): Reads data from an Excel file, prints the value of a cell, and stores data in a 2D array.
Usage
Provide the correct file path in the File object.
The main method reads data from the Excel file specified in the Sheet named "ContactPage."
It prints the value of a cell (family name) and stores the entire sheet data in a 2D array.
2. Class: homePage
Purpose
The homePage class focuses on automated testing of the FreeCRM web application using Selenium and TestNG.

Methods
login(): Sets up the WebDriver, logs into FreeCRM, takes a screenshot, and saves it to a file.
tearDown(): Closes the WebDriver after test execution.
clickContactTests(): Switches to the "Contacts" section of the application.
clickdealsTests(): Switches to the "Deals" section of the application.
clickTasksTests(): Switches to the "Tasks" section, enters keywords and company name for an extended search.
Usage
The login method opens FreeCRM, logs in with predefined credentials, and captures a screenshot.
Three test methods (clickContactTests, clickdealsTests, clickTasksTests) perform specific actions within the FreeCRM application.
3. Class: login
Purpose
The login class contains TestNG test cases for login functionality, URL verification, logo display, and parameterized login tests.

Methods
setUp(): Initializes the WebDriver before each test.
tearDown(): Closes the WebDriver after each test.
litleTest(): Verifies the title of the login screen.
urlCheck(): Verifies the URL of the login screen.
logoTest(): Verifies the display of the CRM logo.
Logintest(String username, String password): Performs login tests with different username and password combinations.
Data Provider
mydata(): Provides data for parameterized login tests.
Conclusion
This Java testing framework integrates Selenium, TestNG, and Apache POI to automate login tests for the FreeCRM web application. It includes functionalities for Excel data handling, capturing screenshots, and parameterized testing. The provided test classes cover various aspects of the application, ensuring robust automated testing capabilities.





