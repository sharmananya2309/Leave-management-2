# Leave Management Portal (Angular + Node.js + MySQL)

A simple leave management portal with separate login views for **HOD** and **Staff**, built using **Angular** for the frontend, **Node.js + Express** for the backend, and **MySQL** for the database.


---

## ✨ Features
###✅Login Page
Login Page allows the user to select their role and enter credentials.

After successful login:
Staff is redirected to their Dashboard.
HOD is redirected to the HOD Dashboard.

🔒 Authentication:
Basic form-based authentication.
User credentials are validated against records in the MySQL users table.
Role-based redirection handled on the frontend using Angular routing.

### 🔐 HOD Panel
- View **Pending** leave requests with **Approve** and **Reject** buttons.
- View **Approved/Rejected** requests (with no action buttons).
- View **History** – past leaves with no pending status.
- Tabs have **active highlighting** when selected.
- UI updated to filter leaves according to current date and status.

### 👩‍💼 Staff Panel
- View leave balance.
- Apply for leave through a form.
- Prevent applying when no leaves are left for a type
- View your leave history.
- View the status of your last leave request 

---

## 📁 Folder Structure
leave-management-2/ 
├── backend/ # Node.js + Express server 
├── frontend/ # Angular frontend 
├── .gitignore 
└── README.md


---

##  How to Run

### Backend (Node.js + Express)

1. Go to the backend folder:
   ```bash
   cd backend
   npm install
   DB_HOST=localhost
   Create a .env file with your DB credentials:
    DB_USER=root
    DB_PASSWORD=yourpassword
    DB_NAME=leave_management
    PORT=5000
   Start the server:
    node index.js

2.Go to the frontend folder:
    cd ../frontend
Install dependencies:
    npm install
Start the Angular dev server:
    ng serve

🛠 Tech Stack
Frontend: Angular, HTML, CSS
Backend: Node.js, Express
Database: MySQL    

Note:
Make sure MySQL server is running and your DB is created.
Use Postman or frontend to test endpoints.
Replace localhost with the server IP in production setup.


🧑‍💻 Author
Ananya Sharma

This project is an enhanced version of my previous React-based leave management system. It introduces additional features and is built using Angular instead of React for the frontend framework.
