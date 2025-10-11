# 🧪 Swag Labs Automation Project

This project automates the functional testing of the **Swag Labs** e-commerce website using **Selenium WebDriver** with **Java** and **TestNG**.  
It validates different user flows such as login, product selection, cart management, checkout, and logout.

---

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Project Structure](#project-structure)
- [Installation & Setup](#installation--setup)
- [How to Run Tests](#how-to-run-tests)
- [Test Reports (Allure)](#test-reports-allure)
- [Jenkins Integration](#jenkins-integration)
- [Technologies Used](#technologies-used)
- [Author](#author)
- [Future Improvements](#future-improvements)

---

## 🧾 Project Overview
The main goal of this project is to provide an automated regression suite for the **Swag Labs** website to ensure all major functionalities are working as expected after each release.

The framework is designed using the **Page Object Model (POM)** structure and follows best practices for code reusability and maintainability.

---

## 📁 Project Structure
```
Swag-Labs-Automation-Project
│
├── src
│   ├── main/java
│   │   └── utilities/            # Helper classes
│   │
│   └── test/java
│       ├── pages/                # Page Object Model classes
│       ├── tests/                # Test classes
│       └── data/                 # Test data files
│
├── pom.xml                       # Maven configuration file
├── testng.xml                    # TestNG suite configuration
├── README.md
└── allure-results/               # Allure results folder (after test execution)
```

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Swag-Labs-Automation-Project.git
   ```

2. **Open the project** in your preferred IDE (IntelliJ IDEA / Eclipse).

3. **Install dependencies** using Maven:
   ```bash
   mvn clean install
   ```

4. **Ensure Java and Maven are installed:**
   ```bash
   java -version
   mvn -version
   ```

---

## ▶️ How to Run Tests

### Run all tests:
```bash
mvn clean test
```

### Run specific TestNG suite:
```bash
mvn test -DsuiteXmlFile=testng.xml
```

### Run from IDE:
- Open `testng.xml`
- Right-click → **Run 'testng.xml'**

---

## 📊 Test Reports (Allure)

After running the tests, Allure results will be generated in:
```
/target/allure-results
```

To view the report:
```bash
allure serve target/allure-results
```

---

## 🤖 Jenkins Integration

This project is configured to run in **Jenkins** as part of a CI/CD pipeline.

Typical Jenkins configuration:
1. **Source Code Management:** Git  
   - Repository URL: `https://github.com/your-username/Swag-Labs-Automation-Project.git`
2. **Build Step:**
   ```bash
   mvn clean test
   ```
3. **Post-build Actions:**
   - Generate **Allure Report**
   - Archive test results

---

## 💻 Technologies Used
- **Java**
- **Selenium WebDriver**
- **TestNG**
- **Maven**
- **Allure Report**
- **Jenkins (CI/CD)**

---

## 👤 Author
**Mo'men Gouda**  
Software Tester (Manual & Automation Testing)  
🔗 [LinkedIn](https://linkedin.com/in/moamn-gouda)

---

## 🚀 Future Improvements
- Add parallel test execution support.
- Integrate API testing.
- Include cross-browser testing using Selenium Grid.
- Add Docker support for containerized execution.

---
