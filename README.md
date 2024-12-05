## Test Automation with Selenium WebDriver
This project is a Java-based automation framework designed to demonstrate test automation using Selenium WebDriver. It includes features like handling multiple browser tabs, interacting with web elements, and generating random test data.

# Project Overview
This test script performs the following actions:

Opens Google in the first browser tab.
Opens a new tab and navigates to an e-commerce website (Tekwill Academy OpenCart).
Automates user registration by generating random user data for fields such as first name, last name, email, and password.
Submits the registration form and validates navigation across multiple browser tabs.
Closes the browser tabs and gracefully exits the WebDriver session.

# Key Features
Selenium WebDriver Integration: Automates interactions with web elements.
Multiple Tab Management: Demonstrates switching between multiple browser tabs using WindowType.TAB.
Random Data Generation: Utilizes RandomDataManager to populate form fields with random but valid data.
JavaScript Execution: Handles actions like scrolling to elements using JavascriptExecutor.
Custom Driver Management: DriverManager simplifies WebDriver setup and management.
# Prerequisites
Before running the project, ensure you have the following installed:

Java JDK 8 or higher
Maven (for dependency management)
A supported WebDriver (e.g., ChromeDriver)
An IDE like IntelliJ IDEA or Eclipse
# Dependencies
The project uses the following libraries:

<dependencies>
    <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>4.x.x</version>
    </dependency>
</dependencies>
Make sure to update the Selenium version in the pom.xml file as needed.

# How to Run
Clone this repository:

git clone https://github.com/Aziz-fer/Java_UI-Automation-Framework.git
cd your-repository
Update the WebDriver path in DriverManager if required.

Build the project using Maven:

mvn clean install
Run the TestRunner class.

mvn exec:java -Dexec.mainClass="com.danacimpoacaqa.TestRunner"
# Project Structure
css
Copy code
src
├── main
│   ├── java
│   │   └── com.danacimpoacaqa
│   │       ├── managers
│   │       │   ├── DriverManager.java
│   │       │   └── RandomDataManager.java
│   │       └── TestRunner.java

# Output
The script outputs the following details to the console:

Current page URLs during navigation.
Randomly generated user email and password for debugging purposes.


# Author
Aziz Feriani
