# Automation-Exercise - Test Automation Framework

**Automation-Exercise** is a robust, modular, and customizable test automation solution designed for both Web Applications and APIs. Built using **Java**, **Selenium**, and **Rest Assured**, this framework adopts industry best practices to ensure scalability, maintainability, and high-performance testing.

## 📝 Description

The project is designed to be modular, allowing easy adaptation to different project requirements. It includes advanced features such as parallel execution, data-driven testing, cross-browser testing, CI/CD integration, and custom reporting.

**Owners:** Mina Khalifa, Adel Elmy  
**Primary Language:** Java

---

## 🚀 Key Features

### Core Capabilities
* **Web Application Testing:** Utilizes **Selenium** for robust and reliable browser automation.
* **API Testing:** Leverages **Rest Assured** for seamless API testing with detailed assertions.
* **Parallel Execution:** Speed up test execution with multi-threading support (TestNG).
* **Cross-Browser Testing:** Compatible with Chrome, Firefox, Edge, and Safari.
* **Data-Driven Testing:** Support for external data sources using **JSON** and **Excel (Apache POI)**.

### Architecture & Design
* **Page Object Model (POM):** Implements POM for better code maintainability and readability.
* **Design Patterns:** Utilizes Singleton, Factory, and Builder patterns for organized code structure.
* **Custom Framework:** Built with reusable components, utilities, and modular architecture.
* **Custom Test Environment:** Support for multiple environments (e.g., dev, staging, production) via properties.

### Reporting & Debugging
* **Allure Reports:** Generates rich HTML reports with detailed execution insights.
* **Evidence Capture:** Automatic screenshots and **video recordings** of test executions.
* **Logs:** Centralized logging using **Log4j** for deep analysis.
* **Custom Listeners:** Enhanced reporting and event logging.

### Resilience
* **Retry Mechanism:** Soft assertions and custom wait strategies to handle flaky tests.
* **CI/CD Integration:** Ready-to-use workflows with **GitHub Actions**.

---

## 🛠️ Tools & Technologies

| Category | Tool/Technology |
| :--- | :--- |
| **Language** | Java (JDK) |
| **Web Automation** | Selenium WebDriver |
| **API Automation** | Rest Assured |
| **Test Runner** | TestNG / JUnit |
| **Build Tool** | Maven / Gradle |
| **Reporting** | Allure Reports |
| **Logging** | Log4j |
| **Data Utilities** | Apache POI (Excel), JSON, Faker (Data Generation) |
| **CI/CD** | GitHub Actions |

---

## 📄 Project Structure

<details>
<summary><strong>Click to view the detailed file tree</strong></summary>

```text
automation-exercise-test/
├── .github/
│   ├── dependabot.yml
│   └── workflows/
│       └── E2E Regression Pipeline.yml
├── .gitignore
├── pom.xml
└── src/
    ├── main/
    │   ├── java/com/automationexercices/
    │   │   ├── FileUtils.java
    │   │   ├── apis/
    │   │   │   ├── Builder.java
    │   │   │   └── UserManagementAPI.java
    │   │   ├── drivers/
    │   │   │   ├── AbstractDriver.java
    │   │   │   ├── Browser.java
    │   │   │   ├── ChromeFactory.java
    │   │   │   ├── EdgeFactory.java
    │   │   │   ├── FirefoxFactory.java
    │   │   │   ├── GUIDriver.java
    │   │   │   ├── SafariFactory.java
    │   │   │   ├── UITest.java
    │   │   │   └── WebDriverProvider.java
    │   │   ├── listeners/
    │   │   │   └── TestNGListeners.java
    │   │   ├── media/
    │   │   │   ├── ScreenRecordManager.java
    │   │   │   └── ScreenshotsManager.java
    │   │   ├── pages/
    │   │   │   ├── CartPage.java
    │   │   │   ├── CheckoutPage.java
    │   │   │   ├── ContactUsPage.java
    │   │   │   ├── DeleteAccountPage.java
    │   │   │   ├── LogoutPage.java
    │   │   │   ├── PaymentPage.java
    │   │   │   ├── ProductDetailsPage.java
    │   │   │   ├── ProductsPage.java
    │   │   │   ├── SignupLoginPage.java
    │   │   │   ├── SignupPage.java
    │   │   │   ├── TestCasesPage.java
    │   │   │   └── components/
    │   │   │       └── NavigationBarComponent.java
    │   │   ├── utils/
    │   │   │   ├── OSUtils.java
    │   │   │   ├── TerminalUtils.java
    │   │   │   ├── TimeManager.java
    │   │   │   ├── WaitManager.java
    │   │   │   ├── actions/
    │   │   │   ├── dataReader/
    │   │   │   ├── logs/
    │   │   │   ├── report/
    │   │   │   └── validations/
    │   └── resources/
    │       ├── META-INF/
    │       ├── allure.properties
    │       ├── db.properties
    │       ├── environment.properties
    │       ├── extensions/
    │       ├── log4j2.properties
    │       ├── seleniumGrid.properties
    │       ├── video.properties
    │       ├── waits.properties
    │       └── webapp.properties
    └── test/
        ├── java/com/automationexercices/tests/
        │   ├── BaseTest.java
        │   ├── api/
        │   │   └── RegisterTestAPI.java
        │   └── ui/
        │       ├── CartTest.java
        │       ├── CheckoutTest.java
        │       ├── InvoiceTest.java
        │       ├── LoginTest.java
        │       ├── PaymentTest.java
        │       ├── ProductDetailsTest.java
        │       ├── ProductsTest.java
        │       └── RegisterTest.java
        └── resources/
            ├── downloads/
            └── test-data/
                ├── cart-data.json
                ├── checkout-data.json
                ├── login-data.json
                ├── product-details-data.json
                ├── products-data.json
                └── register-data.json
