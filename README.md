# 🧹 Online Helping Hand Finder

## 📌 Overview

**Online Helping Hand Finder** is a web-based platform designed to connect clients with domestic workers for everyday household needs. It simplifies the process of finding reliable help by providing a structured interface for **Admins**, **Clients**, and **Domestic Workers** to interact efficiently.

---

## 🎯 Objective

To develop a fully functional website that:
- Connects clients with verified domestic workers
- Allows user registration and secure login
- Enables admins to manage users and services
- Simplifies hiring, tracking, and feedback for household services

---

## 🏠 Core Features

| Role            | Features |
|-----------------|----------|
| **Admin**       | Manage users, view worker/client details, edit database, and review worker experience |
| **Client**      | Hire workers, track previous hires, change password, logout |
| **Worker**      | Manage profile, track clients, update availability, change password |

---

## 🛠️ Technology Stack

- 💻 Frontend: HTML, CSS, JavaScript  
- ⚙️ Backend: ASP.NET / PHP (based on implementation)  
- 🗃️ Database: Microsoft SQL Server  
- 🔐 Authentication: Unique user ID and password for each role  
- 📋 SDLC: Waterfall Model (Requirement → Design → Development → Testing → Deployment)

---

## 🧱 Modules

- 🔐 **User Authentication**  
  Login/registration for Admins, Clients, and Workers

- 🧑‍🔧 **Admin Dashboard**  
  View/edit/delete users, reset passwords, manage categories

- 🧑‍💼 **Client Portal**  
  View available workers, book services, manage history

- 🧑‍🔨 **Worker Panel**  
  Update profile, check job history, manage availability

---

## 📌 Desirable Features

- ✔️ Centralized platform for all domestic service needs  
- ✔️ Category-based filtering of workers  
- ✔️ Real-time availability check  
- ✔️ User-friendly design  
- ✔️ Secure login for all user types  
- ✔️ Unregistered users can browse limited site features  

---

## 🔄 SDLC Model Used: Waterfall

This project follows the **Waterfall Model**, progressing through these stages:

1. Requirements gathering  
2. System design  
3. Implementation (coding)  
4. Testing  
5. Deployment  
6. Maintenance  

The system follows a modular structure with three main user roles: Admin, Client, and Domestic Worker. The interaction and data flow between modules are structured to ensure usability and scalability.

### 📐 General Flow of Waterfall model
<img width="457" alt="General overview of waterfall model" src="https://github.com/user-attachments/assets/94431cd0-cd91-4fb1-8c00-7806bb16c019" />

Data flow diagram is graphical representation of flow of data in an information system. It is capable of depicting incoming data flow, outgoing data flow and stored data. The DFD does not mention anything about how data flows through the system. Data flows are data structures in motion, while data stores are data structures at rest. Hence it is possible that the data flow and the data store would be made up of the same data structure.
### 📐 DFD 0
<img width="347" alt="DFD 0" src="https://github.com/user-attachments/assets/d3fe67e3-24c6-483b-9924-5794242aaf5f" />

### 📐 DFD 1
<img width="353" alt="DFD 1" src="https://github.com/user-attachments/assets/0500bfc6-330c-4431-898b-063dd726c04c" />

### 📊 Entity Relationship Diagram (ERD)

This diagram represents the relationship between Clients, Workers, Admins, and Service Requests.
### 📐 ERD
<img width="348" alt="ERD" src="https://github.com/user-attachments/assets/678cb52f-000a-45d2-892f-1e36a78230e2" />

---

## 🗂️ Data Directory
A detailed description of the admin, client, worker, and hired-by table is depicted.

### 📐 Admin table
<img width="386" alt="admin" src="https://github.com/user-attachments/assets/9123b303-1daf-4c9a-b59c-765a4a67203d" />

### 📐 Client table
<img width="388" alt="client" src="https://github.com/user-attachments/assets/a5b595c4-99f4-44b3-8db2-23377e4d3030" />

### 📐 Worker table
<img width="382" alt="worker" src="https://github.com/user-attachments/assets/dafd27a2-cc18-413f-9410-3d154b79c985" />

### 📐 Hired-by table
<img width="386" alt="hired by" src="https://github.com/user-attachments/assets/89dbf584-ffe6-4cf2-9e72-726b03a7ea40" />

---


## 🧩 System Design 
### 📐 Index/ Home page
This is the landing page of the project. From this index page, we can access other pages linked to it.
![index](https://github.com/user-attachments/assets/0f48cc0e-3256-43e9-9878-de0c985e5ca5)
### 📐 Worker Registration
On clicking the Worker button on the index page, the Worker registration page opens where the worker can register into the database so that the clients can hire them. Workers have to add their unique passwords to access his/her account later.
![workerregis](https://github.com/user-attachments/assets/0db3f6b7-03db-4498-afca-6f42f82dcb51)
### 📐 Client page
On clicking the Client button on the index page, a window opens for the client where they access and visit various categories of workers and can eventually book them. The client needs to be logged in for booking or hiring a worker.
![client](https://github.com/user-attachments/assets/ef1c2211-08c1-41c0-9ccf-dacc4f0c2824)
### 📐 Login page
On clicking the Login button on the index page, a login page opens, where a previously registered client can log in. If a client does not have an account, then they can click on the ‘create an account’ link on the page to open the client registration page. Admin can also log into his account using a secret password which is known to the admin only.
![login](https://github.com/user-attachments/assets/a4f75c7d-5583-4aeb-aaab-09b55a8689af)
### 📐 Admin page
Through this page, admins can view and edit the client and worker databases. On clicking on the view worker button, a page opens which have all the data of the workers stored in a tabular fashion. Again on clicking the view client button, the details of the client can be seen.
![edit](https://github.com/user-attachments/assets/a5548795-3864-4862-9661-d847607b262d)
### 📐 View worker page
This page is only accessible by the Admin. The admin can view the complete list of workers from the database in the table. Admin can edit as well as delete the worker’s entry when needed. 
![viewworker](https://github.com/user-attachments/assets/e09c7464-be68-4cbf-b972-91a3ef7fa168)
### 📐 Update worker page
Admin can update worker’s experiences, job categories, and other data on request from the workers.
![updatew](https://github.com/user-attachments/assets/3b60c01c-09f8-4cf4-b46d-a633f7626370)
### 📐 Worker category page (ex. Carpenter)
There are six different categories of workers in this project namely Carpenter, Plumber, Gardener, Electrician, Driver, and Housekeeper.
![carpenter](https://github.com/user-attachments/assets/51043e1b-be37-4334-9f9a-efbe8b2ce7a6)
### 📐 Service Booking page
When the 'book' button is clicked for an individual worker, the booking page opens up which fetches data of the particular worker from the database and shows it in the text boxes. On clicking the book now button, the client can book their desired worker.
![book](https://github.com/user-attachments/assets/17ce381c-033e-4386-863d-9da126f29cda)
### 📐 Contact-us page
![contactus](https://github.com/user-attachments/assets/c5b514e4-39bc-4b1b-b223-5b998f540870)


---

## 👨‍💻 Authors

- **Debayan Biswas** – [![GitHub](https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white)](https://github.com/deba033)
- **Anirban Dey**
- **Smaranava Roy**
---

## 📄 License

Strictly used for learning purposes. 

