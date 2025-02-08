# 🚍 Futa - Interprovincial Bus Ticket Booking System

## 1️⃣ Introduction
- **Project Name:** Futa – Interprovincial Bus Ticket Booking System 
- **Development Period:** Sep 2024 - Dec 2024
- **Team size:** 03
- **Description:**  
  - A web application that allows users to book bus tickets, select trips, choose seats, and make payments through a user-friendly interface.  
  - The project is built using the Microservices architecture, with Spring Boot for the backend and Next.js for the frontend.  
  - Inspired by **FUTA Bus Lines**.  

---

## 2️⃣ Key features  
✅ Sign up and log in via email or Google  
✅ Search for bus trips by departure and destination points  
✅ View trip details and ticket prices  
✅ Select seats and book tickets  
✅ Make online payments through a payment gateway  
✅ View booking history  
✅ Log out and manage session authentication  


---

## 4️⃣ Architecture diagram 
![image](https://github.com/user-attachments/assets/d1248b14-e1da-41fe-9987-2811c7da1e2d)
---
### **Main components**  

| Component | Description |
|------------|--------------------------------------------------|
| **Client (User)** | Users interact with the system through the Next.js frontend. |
| **API Gateway** | Built using Spring Cloud Gateway, routes requests to the appropriate microservices. It also acts as a load balancer to optimize performance and prevent overload. |
| **Auth Server** | Authentication, using OAuth2 and JWT. |
| **Resource Servers** | Individual microservices, each responsible for a specific function and maintaining its own database. |
| **Eureka Server** | Service Registry helps microservices discovery and register each other. |
| **Swagger** | Provides API documentations for easier testing and development. |
---
### **Feature of each microservice**  

| Microservice | Feature | Tech |
|-------------|----------|-----------|
| **Location Service** | Manages information about bus station, location, city. | Spring Boot, MongoDB |
| **Vehicle Service** | Manages vehicle details such as type, seat layouts, and operational status. | Spring Boot, MySQL |
| **Trip Service** | Manages schedules and trips. | Spring Boot, MongoDB |
| **Booking Service** | Manages ticket booking and invoice processing. | Spring Boot, MySQL |
| **Profile Service** | Manages user profiles and persional information.  | Spring Boot, MySQL |
| **Auth Service** | Handles account management and user authentication. | Spring Boot, OAuth2, JWT, MySQL |
| **Statistic Service** | Collects data from other microservices for reporting and analysis | Spring Boot, Kafka, MongoDB |


---

## 5️⃣ Repositories  
### 🔹 **Backend (Spring Framework)**  
- [`Discovery`](https://github.com/SangNguyenNgoc/booking-trip-discovery) -> Discovery Service and Gateway API
- [`Auth Server`](https://github.com/SangNguyenNgoc/booking-trip-auth) -> Auth Server
- [`Microservices`](https://github.com/SangNguyenNgoc/booking-trip) -> Microservices in application

### 🔹 **Frontend (Next.js)**  
- [`Frontend`](https://github.com/ThanhDat653/futa-client) → UX/UI


---

## 6️⃣ UI   
## Home page
![image](https://github.com/user-attachments/assets/584b6ca9-5c07-4538-bc26-76568860ed56)
## Trip list
![image](https://github.com/user-attachments/assets/0fc851c4-167b-4b3c-baf6-30809e2942f2)
## Select trip & seats
![image](https://github.com/user-attachments/assets/b5990626-9e8f-4171-aba2-6ea7545384c4)
## Seat selection, information review & payment confirmation
![image](https://github.com/user-attachments/assets/e5bc55c9-6132-4d46-ae35-72da55e46648)
## VNPay payment
![image](https://github.com/user-attachments/assets/482b1aa2-a677-4297-9f01-d5b16b331a32)
## Payment successful
![image](https://github.com/user-attachments/assets/84d9f9fe-a704-48e6-951e-7d483cad1986)
## Manage persional & ticket information
![image](https://github.com/user-attachments/assets/044caaaf-c3a0-4274-abd9-b21a900f4cee)
## Ticket lookup
![image](https://github.com/user-attachments/assets/508b9f79-7eb4-4405-84ac-8aad49a78d8c)

---
