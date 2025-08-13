# SkyFleet-Rentals


## 📌 Overview
The **SkyFleet Drone Management System** is a comprehensive platform for managing drone rentals, bookings, and operations.  
It provides role-based access for **Admin** and **Customers**, ensuring secure management of drone services, flight schedules, and booking history.

---

## 🚀 Features
- **User Authentication & Authorization** (JWT Bearer Token)
- **Role-based Access Control** (Admin, User)
- **Drone Inventory Management**
- **Drone Booking & Scheduling**
- **Payment Integration** (Optional)
- **Real-time Status Updates**
- **REST API Endpoints**
- **Responsive UI** (React.js)

---

## 🛠️ Tech Stack
- **Frontend:** React.js, Material-UI, Axios
- **Backend:** Spring Boot, Java 17, Maven
- **Database:** MySQL
- **Authentication:** JWT (Bearer Token)
- **API Testing:** Postman
- **Version Control:** Git & GitHub

---

SkyFleet-Drone/
│── backend/ # Spring Boot REST API
│ ├── src/main/java
│ ├── src/main/resources
│── frontend/ # React.js UI
│ ├── public/
│ ├── src/
│── README.md
│── .gitignore
│── pom.xml # Maven Dependencies
│── package.json # Frontend Dependencies




2️⃣ Backend Setup

mvn clean install
mvn spring-boot:run
3️⃣ Frontend Setup

npm install
npm start

🔑 Authentication
This project uses JWT Bearer Token Authentication.

User logs in with credentials.

Backend generates a JWT token.

Token is sent in Authorization Header for every request:

makefile

Authorization: Bearer <your_token>

📡 API Endpoints (Sample)
Method	Endpoint	Description	Role
POST	/auth/register	Register a new user	Public
POST	/auth/login	Login and get JWT token	Public
GET	/drones	List available drones	User/Admin
POST	/drones	Add a new drone	Admin
POST	/bookings	Book a drone	User

🧪 Testing
Use Postman or cURL to test APIs.
Example:
curl -X GET http://localhost:8080/drones \
-H "Authorization: Bearer <token>"
📜 License
This project is licensed under the MIT License.

👩‍💻 Author
Harshada Tapase
GitHub 
https://github.com/Harshada9595/SkyFleet-Rentals
