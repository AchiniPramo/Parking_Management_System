# 🚗 Smart Parking Management System (SPMS)

A **microservice-based**, cloud-native platform for **real-time parking space management**, built to support smart city initiatives and improve urban mobility.

---

## 🌐 Overview

The **Smart Parking Management System (SPMS)** tackles the growing challenge of urban parking by enabling:

- 🔍 Real-time parking availability tracking
- 🅿️ Reservation & digital space management
- 💳 Secure payment processing
- 📈 Usage analytics by city, zone, and owner

Built using a **Spring Boot microservice architecture**, SPMS supports dynamic scaling, modular deployment, and easy maintainability.

---

## 🧠 Business Objectives

- Allow users to search, reserve, and pay for parking in real time  
- Help parking owners manage and track space usage dynamically  
- Simulate vehicle entry/exit for real-time updates  
- Maintain booking logs for auditing and reporting  
- Reduce traffic congestion and increase parking efficiency  

---

## 🛠️ Technologies & Tools

| Tool/Tech                | Purpose |
|--------------------------|---------|
| **Spring Boot**          | Core framework for all microservices |
| **Spring Cloud Eureka**  | Service discovery and registration |
| **Spring Cloud Gateway** | Central API Gateway |
| **Spring Cloud Config**  | Centralized configuration management |
| **Spring Web**           | REST API development |
| **Postman**              | API testing and validation |
| **Optional:** Node.js / Python Flask | Lightweight services (if needed) |

---

## 🧩 Microservice Architecture

### 1. 🚀 **Service Registry** (Eureka)
- Dynamic service registration & discovery  
- Removes hard-coded dependencies

### 2. ⚙️ **Configuration Server**
- Centralized `application.yml` or `properties` file for all services  
- Dynamic reload without redeployment

### 3. 🌐 **API Gateway**
- Routes client requests to appropriate microservices  
- Leverages Eureka for intelligent routing

### 4. 🧾 **Core Microservices**
| Service | Responsibilities |
|--------|------------------|
| **User Service** | User registration, login, profile, booking history |
| **Parking Space Service** | Manage parking spaces, availability, and reservations |
| **Vehicle Service** | Vehicle registration, entry/exit simulation |
| **Payment Service** | Mock payment flow and digital receipt generation |

---

## 📁 Folder Structure

```

SPMS/
├── user-service/
├── vehicle-service/
├── parking-service/
├── payment-service/
├── eureka-server/
├── config-server/
├── api-gateway/
├── postman\_collection.json
├── docs/
│   └── screenshots/
│       └── eureka\_dashboard.png
└── README.md

````

---

## 📚 Resources

- 📬 [Postman Collection](./Parking_Management_System.postman_collection.json)  
- 📸 ![Eureka Dashboard](./Parking_Management_System\doc\screenshot\eureka_dashboard.png)

---

## 🧪 How to Run the Project

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/SPMS.git
````

2. **Configure database and application properties** in the Config Server repo or folders.

3. **Start Eureka Server**, **Config Server**, and all microservices:

   ```bash
   cd eureka-server
   mvn spring-boot:run
   # Repeat for all services...
   ```

4. **Access Eureka Dashboard**

   ```
   http://localhost:8761
   ```

5. **Test endpoints with Postman** using the provided collection.

---

## 🧑‍💻 Developer

**Achini Pramodhya**
📌 Full Stack Developer | Passionate about Smart Solutions
🔗 [GitHub](https://github.com/your-username)

---

## 📄 License

Distributed under the MIT License. See [`LICENSE`](./LICENSE) for more information.

```

---

Would you like me to also [generate the folder structure](f) or [create your `application.yml` files for each service](f)?
```
