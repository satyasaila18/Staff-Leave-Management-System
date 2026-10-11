# 🏢 Staff Leave Management System

A full-stack web application built with **Python and Django** to manage staff leave requests, authentication, staff accounts, and leave approval workflows.

The system allows staff members to register, log in, apply for leaves, and track their leave requests. Administrators can manage staff accounts and approve or reject leave applications.

---

## 🚀 Features

### 👨‍💼 Staff

- Register an account
- Login and logout
- Access staff dashboard
- Apply for leave
- View submitted leave requests
- Track leave request status

### 👨‍💻 Administrator

- Login as administrator
- Manage staff accounts
- View all leave requests
- Approve leave requests
- Reject leave requests
- Manage staff-related information

---

## 🛠️ Technologies Used

| Technology | Usage |
|---|---|
| Python | Programming Language |
| Django 6.0.5 | Web Framework |
| HTML | Frontend Structure |
| CSS | Styling |
| SQLite | Database |
| Django ORM | Database Operations |
| Django Authentication | User Authentication |

---

## 📂 Project Structure

```text
Staff-Leave-Management-System/
│
├── accounts/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── migrations/
│
├── leave/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   └── migrations/
│
├── slms_project/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── templates/
│   ├── home.html
│   ├── login.html
│   ├── register.html
│   ├── staff_dashboard.html
│   ├── admin_dashboard.html
│   ├── apply_leave.html
│   ├── my_leaves.html
│   ├── view_leaves.html
│   └── accounts/
│
├── manage.py
└── db.sqlite3
⚙️ How It Works

The application is divided into two main Django apps:

accounts

Handles:

User registration
Login and authentication
Staff profiles
Staff/Admin roles
Staff management
leave

Handles:

Leave application
Leave history
Leave request management
Leave approval
Leave rejection

The main project configuration is handled by slms_project.

🔄 Application Flow
User
  │
  ├── Register
  │
  ├── Login
  │
  └── Dashboard
        │
        ├── Staff
        │     ├── Apply Leave
        │     └── View Leave Status
        │
        └── Administrator
              ├── Manage Staff
              ├── View Leave Requests
              ├── Approve Leave
              └── Reject Leave
💻 Installation & Setup
1. Clone the Repository
git clone https://github.com/satyasaila18/Staff-Leave-Management-System.git
2. Navigate to the Project
cd Staff-Leave-Management-System
3. Create a Virtual Environment
python -m venv .venv
4. Activate the Virtual Environment

Windows:

.venv\Scripts\activate

macOS/Linux:

source .venv/bin/activate
5. Install Django
python -m pip install --upgrade pip
pip install "Django==6.0.5"
6. Apply Database Migrations
python manage.py migrate
7. Start the Development Server
python manage.py runserver

Open the application in your browser:

http://127.0.0.1:8000/
🌐 Application URLs
URL	Description
/	Home Page
/register/	User Registration
/login/	Login
/staff_dashboard/	Staff Dashboard
/admin_dashboard/	Administrator Dashboard
/leave/apply_leave/	Apply for Leave
/leave/my_leaves/	View Personal Leave Requests
/leave/view_leaves/	Manage Leave Requests
🗄️ Database

The project currently uses SQLite as its database.

Django ORM is used to interact with the database.

The main data models include:

User
Profile
Leave
🔐 Security & Production Notes

Before deploying the application to production:

Move the SECRET_KEY to environment variables.
Set DEBUG = False.
Configure ALLOWED_HOSTS.
Consider using a production database instead of SQLite.
Avoid committing db.sqlite3.
Add __pycache__/ to .gitignore.
Create a requirements.txt file to document project dependencies.



📌 Future Improvements
Some possible improvements include:

Leave date validation
Email notifications
Password reset functionality
Leave balance tracking
Different types of leave
Improved admin dashboard
Production database support
Automated testing


🎯 Project Purpose
This project was developed to practice and demonstrate:

Python programming
Django web development
Django authentication
Django ORM
CRUD operations
Database management
HTML & CSS
Git & GitHub
👨‍💻 Author

Satya Saila

Computer Science Graduate | Python Developer | AI/ML Enthusiast

🔗 GitHub: github.com/satyasaila18

⭐ If you find this project useful, feel free to explore the repository.


### Small GitHub tip, buddy

Since this is going into your **Staff-Leave-Management-System** repository, I would also create a `.gitignore` so you don't upload `db.sqlite3`, `.venv`, or `__pycache__`.

A good one for this project is:

```gitignore
.venv/
__pycache__/
*.pyc
db.sqlite3
.env

Then:

git add .
git commit -m "Add project README and gitignore"
git push

This will keep your Django repository much cleaner. 🚀
