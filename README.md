
#  Scalable Tourism Management System  

A **microservices-based tourism booking platform** built by me and my team.  
This project simplifies hotel and room booking operations while ensuring **scalability, fault tolerance, and maintainability**.  

---

## 📊 Tech Stack  

![Java](https://img.shields.io/badge/Java-17-orange?logo=openjdk)  
![Spring Boot](https://img.shields.io/badge/SpringBoot-3.x-green?logo=springboot)  
![MySQL](https://img.shields.io/badge/MySQL-8-blue?logo=mysql)  
![Hibernate](https://img.shields.io/badge/Hibernate-ORM-yellow)  
![Docker](https://img.shields.io/badge/Docker-Enabled-blue?logo=docker)  

---

## 🚀 Why Microservices?  

- **Scalability** → Each service runs independently.  
- **Load Balancing** → Spring Cloud Gateway ensures smooth traffic distribution.  
- **Service Discovery** → Eureka auto-registers services, reducing config overhead.  
- **Flexibility** → Add more services (Payment, Reviews, Notifications) without touching existing ones.  

---

## 🏗️ Architecture  

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

## 📂 Features  

- 👤 **Admin Module** → Add/admins, manage hotels, requests, customers.  
- 🏨 **Hotel Management** → Add hotels, update rooms, retrieve details.  
- 📅 **Booking System** → Book/cancel rooms, search by date, check availability.  
- 🙍 **Customer Module** → Registration, booking history, cancellations.  
- 📩 **Request Handling** → Submit/view/cancel service requests.  

---

## 🛠️ How to Run  

1️⃣ Clone repo  
```bash
git clone https://github.com/RAGHVENDRA04/Scalable-Tourism-Management-System.git
cd Scalable-Tourism-Management-System
````

2️⃣ Start Eureka Server

```bash
cd TourismEureka-tourism
mvn spring-boot:run
```

3️⃣ Start API Gateway

```bash
cd TourismApiGateway-tourism
mvn spring-boot:run
```

4️⃣ Run Microservices

```bash
cd Service1 && mvn spring-boot:run
cd Service2 && mvn spring-boot:run
```

5️⃣ Test APIs (Postman)

* `POST /addhotel`
* `POST /addbooking`
* `GET /findhotel`

---

## ✨ Future Enhancements

* 💳 Add **Payment Service** (Stripe/PayPal)
* ⭐ Add **Reviews & Ratings** for hotels
* 🎨 Build a **React Frontend**
* 🐳 Deploy with **Docker Compose**

---

## 🤝 Contributing

Fork → Branch → Commit → PR.
Contributions are welcome in: new services, better security, frontend UI.

---

## 📜 Copyright

© 2025 **Raghvendra Singh**. All rights reserved.
Published for **learning & demonstration** purposes.



👉 Want me to also design a **graphical architecture diagram** (colored PNG flow) that you can embed directly into the README instead of ASCII? That’ll make it pop even more.
```
