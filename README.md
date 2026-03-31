

---

# 📘 3. SERVICES README  
👉 (student / program / enrollment)

```md
# 🧩 Microservices (Student, Program, Enrollment)

## 👩‍🎓 Student Information

- **Student Name**: M.A. Nethranjali Jayasanki  
- **Student ID**: 2301691109  
- **GCP Project ID**: capstone-project-491809 

---

## 📌 Project Description

This repository contains the **business microservices** of the system.

Each service is independently deployable and communicates through the API Gateway.

---

## 📦 Services

- Student Service  
- Program Service  
- Enrollment Service  

---

## 🔗 Integration

Each service:

- Registers with Eureka  
- Uses Config Server  
- Accessed via API Gateway  

---

## 🚀 API Access

Base URL:

http://34.36.72.235


---

## 🗄️ Database

✔ Relational DB (MySQL / PostgreSQL)  
✔ Non-relational DB (MongoDB)  

---

## 🔄 PM2 Execution

```bash
pm2 start "java -jar target/*.jar" --name student-service
pm2 start "java -jar target/*.jar" --name program-service
pm2 start "java -jar target/*.jar" --name enrollment-service
pm2 save
