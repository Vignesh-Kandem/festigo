# 🎉 Festigo – Community Event Platform

Festigo is a full-stack web application designed to simplify **event discovery, booking, and management**.
It enables users to explore and book events, while organizers can create and manage events efficiently.

---

## 🚀 Features

### 👤 User Features

* 🔐 User Registration & Login
* 📅 Browse Available Events
* 🎟 Book Events
* 📌 View Booked Events
* 📝 Submit Reviews (Blog Section)

### 🧑‍💼 Organizer Features

* 🔐 Organizer Login
* ➕ Create Events
* ✏ Edit Events
* ❌ Delete Events
* 👥 Manage Participants

---

## 🛠️ Tech Stack

### 🌐 Frontend

* HTML5
* CSS3 (Glassmorphism UI)
* JavaScript
* Jinja2 Templates

### ⚙️ Backend

* Python (Flask)
* Flask Routing & Session Management

### 🗄️ Database

* SQLite (Deployment)
* MYSQL (Development)
* SQLAlchemy ORM

### 🔐 Authentication

* Werkzeug Security (Password Hashing)

---

## 📂 Project Structure

```
festigo/
│
├── static/                # CSS, Images
├── templates/             # HTML Templates
│
├── app.py                 # Main Flask Application
├── requirements.txt       # Dependencies
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/festigo.git
cd festigo
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # (Linux/Mac)
venv\Scripts\activate      # (Windows)
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run Application

```bash
python app.py
```

👉 Open in browser:

```
http://127.0.0.1:5000
```

---

## 🧠 Workflow Overview

The platform follows a structured workflow:

### 👤 User Flow

1. Register/Login
2. Browse Events
3. Book Event
4. View Bookings
5. Submit Review

### 🧑‍💼 Organizer Flow

1. Login
2. Access Dashboard
3. Create/Edit/Delete Events
4. Manage Participants

### 🗄️ Backend Flow

* All data stored in database
* No email notifications used
* No payment integration

---

## 🧾 Database Design

### Users Table

* user_id
* user_name
* user_email
* user_password
* user_role

### Events Table

* event_id
* event_title
* event_description
* event_date
* location
* created_by
* event_seats
* event_price

### Registrations Table

* registration_id
* participant_id
* event_ref_id

### Blog (Reviews) Table

* blog_id
* registration_id
* review

---

## ⚠️ Limitations

* ❌ No payment gateway
* ❌ No email notifications
* ❌ SQLite not suitable for production

---

## 🚀 Future Enhancements

* 💳 Payment Integration
* 📧 Email Notifications
* 📊 Admin Dashboard
* 📱 Mobile Responsive Improvements
* 🌍 Deploy with PostgreSQL
* 🤖 LLM Integration with GPT's
