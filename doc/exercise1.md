# Exercise 1 - Spring Boot Application

## 📌 Overview
This project is a **Spring Boot** application developed as part of the Agile Techniques course. It is designed to provide a set of basic functionalities through a web interface, following the **Model-View-Controller (MVC) architecture**. The application is containerized using **Docker** and includes automated testing to ensure functionality and reliability.

## 🚀 Implemented Functionalities
The application includes the following features:

### **Palindrome Checker**
Allows users to input a word or phrase and determines whether it is a palindrome, ignoring spaces and case sensitivity.
- **Controller:** Handles HTTP requests and forwards user input to the service layer.
- **Service:** Implements logic to strip spaces and check if the string is identical when reversed.
- **Thymeleaf View:** Displays input and results.

### **Even Number Checker**
Determines if an entered number is even or odd.
- **Controller:** Processes requests and passes the number to the service layer.
- **Service:** Uses simple modulus operation to determine if the number is even.
- **Thymeleaf View:** Displays the result to the user.

### **Basic Calculator**
Performs basic arithmetic operations including addition, subtraction, multiplication, and division.
- **Controller:** Accepts numerical inputs and the desired operation.
- **Service:** Implements logic for mathematical calculations and handles division by zero cases.
- **Thymeleaf View:** Provides an interactive form for users to enter numbers and select operations.

### **Square Number Checker**
Checks if one number is the square of another.
- **Controller:** Receives two numbers and passes them to the service.
- **Service:** Computes if the first number squared equals the second number.
- **Thymeleaf View:** Displays the result and allows user re-entry.

---

## 🛠️ Implementation Details
The project was implemented using:
- **Spring Boot:** Framework for Java web applications.
- **Thymeleaf:** Template engine for rendering views.
- **Maven:** Dependency management and build automation tool.
- **JUnit & MockMvc:** Automated testing tools.
- **Docker:** Containerization for easy deployment.

Each functionality follows a structured approach:
- **Controller Layer:** Manages HTTP requests and directs traffic.
- **Service Layer:** Contains the core logic and computations.
- **View Layer:** Uses Thymeleaf templates to present results.

---

## ✅ Testing
The project includes **unit tests and integration tests** to verify correctness and stability.

### 🔹 **Unit Tests**
- **Service Layer Tests:** Validate that each service method functions correctly.
- **JUnit Assertions:** Verify expected versus actual outcomes.

### 🔹 **Integration Tests**
- **MockMvc Tests:** Simulate HTTP requests and verify responses.
- **Form Input Handling:** Ensure correct parsing of user input.

To run all tests, execute:
```bash
mvn test
```

---

## 🌐 Project Repositories
- **GitHub Repository:**  
  👉 [https://github.com/acoves/p1-springboot-app-ATSD](https://github.com/acoves/p1-springboot-app-ATSD)

- **DockerHub Image:**  
  👉 [https://hub.docker.com/r/acoves/spring-boot-demoapp](https://hub.docker.com/r/acoves/spring-boot-demoapp)

To pull and run the Docker image:
```bash
docker pull acoves/spring-boot-demoapp:latest
docker run -p 8080:8080 acoves/spring-boot-demoapp
```

---

## 📌 Conclusion
This project demonstrates the **use of Spring Boot with MVC architecture, automated testing with JUnit and MockMvc, and containerization with Docker**. The application is fully functional and tested, ensuring robustness and usability. The modular implementation ensures scalability and maintainability for future enhancements.

If you have any suggestions or improvements, feel free to contribute to the repository! 🚀
