# Automation-Selenium-Framework

## Overview
This project is a Selenium-based automation testing framework built with Java and TestNG. It provides a structured approach for automating web application testing, including browser management, test execution, and reporting.

## Features
- Selenium WebDriver integration
- TestNG for test management
- Page Object Model (POM) design pattern
- Easy browser setup and teardown
- Extensible base test class
- Sample test cases and suites

## Prerequisites
- Java JDK 8 or higher
- Maven
- Chrome browser
- ChromeDriver (ensure the version matches your Chrome browser)
- Eclipse IDE (recommended)

## Project Structure
```
Automation-Selenium-Framwork/
├── pom.xml
├── testing.xml
├── src/
│   ├── main/
│   │   └── java/
│   │       └── base/
│   │           └── BaseTest.java
│   └── test/
│       └── ... (your test classes)
├── target/
│   └── ... (build output)
└── test-output/
    └── ... (TestNG reports)
```

## How to Run
1. **Clone the repository**
2. **Install dependencies:**
   - Open a terminal in the project root and run:
     ```
     mvn clean install
     ```
3. **Run tests:**
   - Execute all tests using TestNG suite:
     ```
     mvn test -DsuiteXmlFile=testing.xml
     ```
   - Or run individual test classes from Eclipse/TestNG.

## Configuration
- **BaseTest.java**: Handles browser setup and teardown.
- **testing.xml**: TestNG suite configuration file.
- **pom.xml**: Maven dependencies and build configuration.

## Adding New Tests
1. Create a new test class in `src/test/java/`.
2. Extend `base.BaseTest` for browser management.
3. Annotate your test methods with `@Test`.
4. Add your test class to `testing.xml` if you want it included in the suite.

## Reporting
- TestNG generates HTML reports in the `test-output/` directory after test execution.

## Troubleshooting
- Ensure ChromeDriver is compatible with your Chrome browser version.
- If tests fail to start, check your WebDriver path and browser installation.
- For Maven issues, run `mvn clean` and then `mvn install`.

## License
This project is for educational and demonstration purposes.
