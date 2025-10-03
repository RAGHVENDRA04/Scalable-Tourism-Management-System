
# 🌍 Scalable Tourism Management System  

A **microservices-based tourism booking platform** built during my internship at **ThunderCube Pvt. Ltd.**  
This project simplifies hotel and room booking operations while ensuring **scalability, fault tolerance, and maintainability**.  

---

## 📊 Tech Stack Overview  

```

Backend (Java + Spring Boot)   ██████████ 40%
Database (MySQL + Hibernate)   ██████ 25%
API Gateway + Eureka           ████ 20%
Frontend (HTML, CSS, JS)       ██ 10%
Docker & Deployment            █ 5%

```

---

## 🚀 Why Microservices?  

Instead of a monolithic design, this project follows a **microservices architecture** because:  

- **Scalability** → Each service (Hotel, Booking, Customer, Admin) runs independently.  
- **Load Balancing** → Requests are evenly distributed with **Spring Cloud Gateway**.  
- **Service Discovery** → New services auto-register with **Eureka**, no manual config needed.  
- **Flexibility** → Additional services (e.g., *Payment Service*, *Review Service*) can be added without breaking the system.  

---

## 🏗️ Project Architecture  

```

[ Client ]
↓
[ API Gateway ] → [ Eureka Registry ]
↓
┌─────────────┐       ┌─────────────┐
│  Service 1  │       │  Service 2  │
│ (Customer & │       │  (Admin &   │
│  Booking)   │       │   Hotels)   │
└─────────────┘       └─────────────┘

````

---

## 📂 Features Implemented  

✅ **Admin Module** → Add/authenticate admins, manage customers, hotels, and requests.  
✅ **Customer Module** → Register, book rooms, cancel bookings, view history.  
✅ **Hotel Management** → Add hotels, update rooms, fetch hotel info.  
✅ **Booking System** → Date-based search, availability checks, cancellations.  
✅ **Request Handling** → Submit, view, and cancel requests.  

---

## 🛠️ How to Run  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/RAGHVENDRA04/Scalable-Tourism-Management-System.git
cd Scalable-Tourism-Management-System
````

### 2️⃣ Start Eureka Server

```bash
cd TourismEureka-tourism
mvn spring-boot:run
```

### 3️⃣ Start API Gateway

```bash
cd TourismApiGateway-tourism
mvn spring-boot:run
```

### 4️⃣ Run Microservices

```bash
cd Service1
mvn spring-boot:run

cd Service2
mvn spring-boot:run
```

### 5️⃣ Test APIs with Postman

Example endpoints:

* `POST /addhotel`
* `POST /addbooking`
* `GET /findhotel`

---

## ✨ Future Enhancements

🔹 Add **Payment Service** (Stripe/PayPal integration)
🔹 Add **Review & Rating Service** for hotels
🔹 Build a **React Frontend** for modern UI
🔹 Containerize all services with **Docker Compose**

---

## 🤝 Contributing

Contributions are welcome 🎉

* Fork the repo
* Create a feature branch
* Commit your changes
* Submit a PR

Open areas:

* New microservices
* Security improvements
* Frontend UI

---

## 📜 Copyright

© 2025 **Raghvendra Singh**. All rights reserved.
This project is published for **learning and demonstration purposes**.

---

```

---

🔥 This version is:  
- **Professional & GitHub-ready** (clear sections, visuals, diagrams).  
- Humanized with explanations and reasoning.  
- Organized with step-by-step guidance.  
- Leaves room for contributors.  

👉 Do you want me to **add shields.io badges** (Java, Spring Boot, MySQL, GitHub stars, forks) at the top so your README looks even more attractive like open-source repos?
```
