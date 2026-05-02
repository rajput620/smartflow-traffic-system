# 🚦 SmartFlow Traffic Management System (Spring Boot)

## 📌 Overview

SmartFlow Traffic Management System is a **Spring Boot-based web application** that simulates and manages real-time traffic flow. It processes vehicle data such as speed, zone, and status to control traffic signals dynamically and detect congestion or priority conditions.

---

## 🏗️ Project Architecture

This project follows a standard **Spring Boot MVC architecture**:

* **Controller Layer**

  * `TrafficController.java` → Handles traffic-related logic
  * `PageController.java` → Manages page routing

* **Service Layer**

  * Business logic for processing traffic conditions

* **Repository Layer**

  * Data handling (can be extended for database integration)

* **Model**

  * `TrafficData.java` → Represents vehicle and traffic data

* **Frontend**

  * `index.html` (Thymeleaf template)

---

## 📂 Project Structure

```bash
smartflow-traffic-ui/
│── src/main/java/com/smartflow/
│   ├── controller/
│   │   ├── PageController.java
│   │   └── TrafficController.java
│   ├── model/
│   │   └── TrafficData.java
│   ├── repository/
│   ├── service/
│   └── SmartFlowApplication.java
│
│── src/main/resources/
│   ├── templates/
│   │   └── index.html
│   └── application.properties
│
│── pom.xml
│── mvnw / mvnw.cmd
│── Dockerfile
│── target/
```

---

## ✨ Features

* 🚗 Vehicle data input (ID, speed, zone)
* 📍 Zone-based traffic classification (City, Highway, Hospital)
* 🚦 Dynamic signal control (Red / Green)
* ⚠️ Traffic condition detection (Normal / Overload / Priority)
* 🚑 Emergency vehicle handling
* 📊 Real-time table and chart visualization
* 🔄 Add, process, refresh, and clear operations

---

## 🛠️ Tech Stack

* **Backend:** Spring Boot (Java)
* **Frontend:** HTML, CSS, JavaScript (Thymeleaf)
* **Build Tool:** Maven
* **Containerization:** Docker

---

## 🚀 How to Run the Project

### 1. Clone Repository

```bash
git clone https://github.com/your-username/smartflow-traffic-ui.git
cd smartflow-traffic-ui
```

### 2. Run using Maven Wrapper

```bash
./mvnw spring-boot:run
```

*(Windows)*

```bash
mvnw.cmd spring-boot:run
```

### 3. Open in Browser

```
http://localhost:8080
```

---

## 🐳 Run with Docker

```bash
docker build -t smartflow .
docker run -p 8080:8080 smartflow
```

---

## ⚙️ How It Works

1. User inputs vehicle details via UI.
2. Backend processes traffic data.
3. System determines:

   * **Normal Flow**
   * **Overload Condition**
   * **Emergency Priority**
4. Traffic signals update dynamically.
5. Results are displayed in table and chart.

---

## 🔮 Future Enhancements

* Integration with real-time traffic APIs
* AI-based traffic prediction
* Database support (MySQL/PostgreSQL)
* Live GPS tracking
* Multi-intersection traffic control

---

## 📄 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

**Gaurav Singh Rajput**
