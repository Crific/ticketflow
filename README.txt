# TicketFlow

A modern support ticket management web application built with Flask.

TicketFlow is a full-stack CRUD web application designed for managing support requests, internal operations tickets, and workflow tracking through a clean role-based system.

---

# Features

## Authentication System

* User registration and login
* Secure password hashing using Werkzeug
* Session-based authentication with Flask-Login
* Logout protection using POST requests
* Input validation and duplicate account prevention

## User Dashboard

* Create support tickets
* Edit existing tickets
* Delete tickets
* Track ticket statuses
* View ticket priority levels
* Personalized dashboard experience

## Admin Dashboard

* View all submitted tickets
* Update ticket statuses
* Priority-based ticket sorting
* Separate admin-only dashboard access
* Manage internal workflow requests

## Ticket Management

* Ticket title and description system
* Priority levels:

  * High
  * Medium
  * Low
* Status tracking:

  * Pending
  * In Progress
  * Completed
* Organized ticket card layout

## UI / UX

* Responsive dashboard layout
* Clean modern interface
* Flash message feedback system
* Reusable dashboard card structure
* Consistent styling across pages
* Role-based homepage rendering

---

# Tech Stack

## Backend

* Python
* Flask
* Flask-Login
* Flask-SQLAlchemy
* SQLite

## Frontend

* HTML
* CSS
* Jinja2 Templates

## Development Tools

* VS Code
* Git
* GitHub

---

# Project Structure

```bash
TicketFlow/
│
├── app.py
├── requirements.txt
├── users.db
│
├── static/
│   ├── style.css
│   └── auth.css
│
├── templates/
│   ├── home.html
│   ├── login.html
│   ├── register.html
│   ├── dashboard.html
│   ├── admin_dash.html
│   ├── admin_ticket.html
│   ├── create_ticket.html
│   ├── edit_ticket.html
│   └── profile.html
│
└── README.md
```

---

# Database Models

## User

| Field    | Type    |
| -------- | ------- |
| id       | Integer |
| username | String  |
| email    | String  |
| password | String  |
| role     | String  |

## Request

| Field    | Type    |
| -------- | ------- |
| id       | Integer |
| user_id  | Integer |
| title    | String  |
| body     | Text    |
| priority | String  |
| status   | String  |

---

# Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/ticketflow.git
cd ticketflow
```

## Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Mac/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

---

# Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Run Application

```bash
python app.py
```

Application will run on:

```bash
http://127.0.0.1:5000
```

---

# Future Improvements

* Ticket replies/comments
* File attachments
* Search and filtering
* Email notifications
* Analytics dashboard
* API integration
* Dark mode
* Deployment pipeline

---

# Screenshots

Add screenshots here after deployment.

Examples:

* Login Page
* Dashboard
* Admin Dashboard
* Ticket View
* Ticket Creation Form

---

# Learning Goals

This project was built to strengthen:

* Full-stack web development fundamentals
* CRUD application architecture
* Authentication systems
* Database relationships
* Flask routing and templates
* UI structure and responsive layouts
* Role-based access control
* Real-world project organization

---

# Author

Justin Isidro

GitHub: [https://github.com/Crific](https://github.com/Crific)

---

# License

This project is open-source and available for learning and portfolio purposes.
