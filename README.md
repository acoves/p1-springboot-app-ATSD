# Spring Boot Application - Agile Techniques

This application was developed using **Spring Boot** and **Thymeleaf** as part of the **Agile Techniques** course.  
It includes multiple interactive features accessible through a web interface.

## 🚀 Implemented Features

The application allows performing the following operations:

🏠 **Palindrome Checker** – Checks if a word or phrase is a palindrome.  
🏠 **Even Number Checker** – Determines if an entered number is even.  
🏠 **Calculator** – Performs basic mathematical operations (addition, subtraction, multiplication, and division).  
🏠 **Square Checker** – Verifies if a number is the square of another.

Each feature has its own form where the user can input data and view the results.

---

## 📌 Requirements

To run the application, you need:

- **Java 8 or later**
- **Maven** (included in the project with `mvnw`)

---

## 🏃 Running the Application

### **Run with Maven**
You can run the application directly using the _goal_ `run` from the Spring Boot Maven _plugin_:

```bash
./mvnw spring-boot:run
```

### **Build and Run a JAR**
If you prefer to package the application into a **JAR file** and run it manually:

```bash
./mvnw package
java -jar target/demoapp-0.0.1-SNAPSHOT.jar
```

---

## 🌐 Accessing the Application

Once the application is running, access these routes from a browser:

- **Home Page:**  
  [http://localhost:8080](http://localhost:8080)
- **Personalized Greeting:**  
  [http://localhost:8080/saludoform](http://localhost:8080/saludoform)
- **Palindrome Checker:**  
  [http://localhost:8080/palindrome](http://localhost:8080/palindrome)
- **Even Number Checker:**  
  [http://localhost:8080/evenNumber](http://localhost:8080/evenNumber)
- **Calculator:**  
  [http://localhost:8080/calculator](http://localhost:8080/calculator)
- **Square Checker:**  
  [http://localhost:8080/square](http://localhost:8080/square)

---

## 🐳 Running with Docker

The application is also available as a **Docker image** on DockerHub.

### **1️⃣ Pull the image from DockerHub**
```bash
docker pull acoves/spring-boot-demoapp:latest
```

### **2️⃣ Run the image in a container**
```bash
docker run -p 8080:8080 acoves/spring-boot-demoapp
```

Then access the application at [http://localhost:8080](http://localhost:8080).

---

## 📂 GitHub Repository

The source code is available on GitHub:

👉 **Repository:** [https://github.com/acoves/p1-springboot-app-ATSD](https://github.com/acoves/p1-springboot-app-ATSD)

---

## 🛠️ DockerHub Image

You can get the preconfigured image from DockerHub:

👉 **DockerHub:** [https://hub.docker.com/r/acoves/spring-boot-demoapp](https://hub.docker.com/r/acoves/spring-boot-demoapp)

👉 **Public View of the Final Image:** [https://hub.docker.com/r/acoves/spring-boot-demoapp/tags](https://hub.docker.com/r/acoves/spring-boot-demoapp/tags)

---

## ✅ Automated Testing

Unit and integration tests have been implemented to ensure the correct functionality of the application.  
To run the tests:

```bash
mvn test
```

Includes:
- **Service tests:** Validate all mathematical operations, verifications, and conversions.
- **Integration tests with MockMvc:** Ensure controllers return the correct views and handle data properly.

---

## 📑 Practice Documentation

All detailed documentation is available in:

📚 **File:** `doc/exercise1.md`

---

## 🎯 Conclusion

This application was developed using the **MVC pattern in Spring Boot**, implementing automated tests with **JUnit and MockMvc**.  
It has been optimized for local execution and Docker container deployment.

If you have any questions or suggestions, feel free to contribute to the repository. 🚀😃
