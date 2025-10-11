# 🧪 Swag Labs Automation Project

## 📋 Overview
This project automates end-to-end testing for the **Swag Labs** web application using **Selenium WebDriver**, **TestNG**, and **Java**.  
The project follows the **Page Object Model (POM)** design pattern for better maintainability and scalability.  
Reports are generated using **Allure** and the project is integrated with **Jenkins** for CI/CD.

---

## 🧰 Tools & Technologies
- **Java:** Core language used for writing test automation scripts.  
- **Selenium WebDriver:** Browser automation for web application testing.  
- **TestNG:** Test case structuring, execution, and reporting.  
- **Maven:** Dependency management and build automation.  
- **Log4j:** Centralized logging for better debugging and analysis.  
- **Allure Reports:** Rich HTML reports with execution insights.  
- **Faker:** Generate fake data for testing purposes.  
- **JSON:** Used for test data and configuration.  
- **Jenkins / GitHub Actions:** CI/CD integration for automated testing and report generation.  

---

## 🧩 Project Structure

```
src
 ┣ java
 ┃ ┣ DriverFactory
 ┃ ┃ ┗ DriverFactory.java
 ┃ ┣ Pages
 ┃ ┃ ┣ P01_LoginPage.java
 ┃ ┃ ┣ P02_LandingPage.java
 ┃ ┃ ┣ P03_CartPage.java
 ┃ ┃ ┣ P04_CheckoutPage.java
 ┃ ┃ ┣ P05_OverviewPage.java
 ┃ ┃ ┗ P06_FinishingOrderPage.java
 ┃ ┣ Utilities
 ┃ ┃ ┣ DataUtils.java
 ┃ ┃ ┣ LogsUtils.java
 ┃ ┃ ┗ Utility.java
 ┃
 ┣ test
 ┃ ┣ Listeners
 ┃ ┃ ┣ InvokedMethodListenerClass.java
 ┃ ┃ ┗ ITestResultListenerClass.java
 ┃ ┣ Tests
 ┃ ┃ ┣ TC01_LoginTest.java
 ┃ ┃ ┣ TC02_LandingTest.java
 ┃ ┃ ┣ TC03_CartTest.java
 ┃ ┃ ┣ TC04_CheckoutTest.java
 ┃ ┃ ┣ TC05_OverviewTest.java
 ┃ ┃ ┗ TC06_FinishingOrderTest.java
 ┗ resources
```

---

## 🚀 How to Run Tests

1. Clone the repository  
   ```bash
   git clone https://github.com/Moamngouda/Swag-Labs-Automation-Project.git
   ```

2. Navigate to the project directory  
   ```bash
   cd Swag-Labs-Automation-Project
   ```

3. Run tests using Maven  
   ```bash
   mvn clean test
   ```

4. Generate Allure Report  
   ```bash
   allure serve allure-results
   ```

---

## 🧩 Prerequisites
Before running the project, make sure you have:
- **Java Development Kit (JDK)** installed  
- **IDE** (e.g., IntelliJ IDEA, Eclipse)  
- **Maven** installed  
- **Allure Commandline** installed (for viewing reports)  

---

## 🧾 Test Reporting
After test execution, Allure will generate HTML reports located in:
```
/target/allure-results
```
To view reports locally:
```
allure serve target/allure-results
```

---

## 🧱 Continuous Integration (Jenkins)
This project can be integrated with **Jenkins** using a `Pipeline` or `Freestyle` job.  
It runs automatically on each push or pull request and generates **Allure reports** for each build.

---

## 👤 Author
**Mo'men Gouda**  
Junior Quality Control Engineer 
🔗 [LinkedIn](https://www.linkedin.com/in/mo-men-gouda-0b060a284/)

---

