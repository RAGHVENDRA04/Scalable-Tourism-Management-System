"# Scalable-Tourism-Management-System" 
# 🌍 Scalable Tourism Management System  

A **microservices-based tourism booking platform** built during my internship at ThunderCube Pvt. Ltd. This project simplifies hotel and room booking operations while ensuring scalability, fault tolerance, and maintainability.

---

## 📊 Tech Stack Overview  

Backend (Java + Spring Boot) ██████████ 40%
Database (MySQL, Hibernate) ██████ 25%
API Gateway + Eureka ████ 20%
Frontend (HTML, CSS, JS) ██ 10%
Docker & Deployment █ 5%

yaml
Copy code

---

## 🚀 Why Microservices?  
I used **microservices** instead of a monolith because:  
- **Scalability:** Each service (hotel, booking, customer, admin) runs independently.  
- **Load Balancing:** With Spring Cloud Gateway, requests are distributed smoothly.  
- **Service Discovery:** Eureka ensures new services auto-register without manual config.  
- **Flexibility:** You can add more services later (e.g., `Payment Service`, `Review Service`) without breaking existing code.  

---

## 🏗️ Project Architecture  

[ Client ] → [ API Gateway ] → [ Eureka Registry ]
| |
┌────────┴────────┐ ┌─────┴─────┐
[ Service1 ] [ Service2 ] ... add more
(Customer/Booking) (Admin/Hotel)

yaml
Copy code

---

## 📂 Features Implemented  

- **Admin Module** → Add/Authenticate Admins, manage customers, hotels, and requests.  
- **Customer Module** → Register, book rooms, cancel bookings, view history.  
- **Hotel Management** → Add hotels, update rooms, retrieve hotel info.  
- **Booking System** → Date-based search, availability check, and cancellations.  
- **Request Handling** → Track customer requests with APIs.  

---

## 🛠️ How to Run  

### 1️⃣ Clone the repo  
```bash
git clone https://github.com/RAGHVENDRA04/Scalable-Tourism-Management-System.git
cd Scalable-Tourism-Management-System
2️⃣ Start Eureka Server
bash
Copy code
cd TourismEureka-tourism
mvn spring-boot:run
3️⃣ Start API Gateway
bash
Copy code
cd TourismApiGateway-tourism
mvn spring-boot:run
4️⃣ Run Microservices
bash
Copy code
cd Service1
mvn spring-boot:run

cd Service2
mvn spring-boot:run
5️⃣ Test APIs with Postman
Endpoints like:

POST /addhotel

POST /addbooking

GET /findhotel

✨ Future Enhancements
Add Payment Service (Stripe/PayPal integration).

Add Review & Rating Service for hotels.

Build a React Frontend for modern UI.

Containerize everything with Docker Compose.

🤝 Contributing
Want to improve this project? Fork the repo, create a feature branch, and submit a PR.
I’m open to contributions around new services, better security, or frontend UI.

📜 Copyright
© 2025 Raghvendra Singh. All rights reserved.
This project is published for learning and demonstration purposes.

pgsql
Copy code

---

🔥 This README is structured, visual, and **looks like a real human project** (not auto-generated). It shows your **skills, reasoning, diagrams, and usage instructions** clearly.  

👉 Do you want me to also create **badges (GitHub stars, forks, tech logos like Java, Spring Boot, MySQL)** to make the READ
