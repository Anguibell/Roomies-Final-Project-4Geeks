# 🏠 Roomies – Full Stack University Roommate Matching Platform

![Python](https://img.shields.io/badge/Python_3.10-3776AB?style=flat&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat&logo=sqlalchemy&logoColor=white)
![React](https://img.shields.io/badge/React.js-20232A?style=flat&logo=react&logoColor=61DAFB)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase_%2F_Firestore-FFCA28?style=flat&logo=firebase&logoColor=black)

## 📌 Project Overview
**Roomies** is a full-stack web application designed to help university students search, filter, and match with compatible roommates and housing options based on customized lifestyle, budget, and location criteria.

Developed as the Capstone Project for the **360-hour Full Stack Software Developer Bootcamp at 4Geeks Academy**.

---

## 🚀 Key Features & Architecture
- **Smart Roommate & Property Filtering:** Custom search engine allowing students to filter housing listings and roommate profiles by preferences and budget.
- **RESTful Backend API (Python & Flask):** Modular backend handling authentication, user profiles, property listings, and matching preferences.
- **Relational Database Abstraction (SQLAlchemy & PostgreSQL):** Structured relational schema with automated migration management and custom CLI seed commands.
- **Real-Time Data & Cloud Integration (Firebase / Firestore):** Dynamic updates for user interactions and real-time platform synchronization.
- **Responsive Single-Page Frontend (React.js):** Modern component-based UI bundled with Webpack.

---

## 🛠️ Tech Stack
- **Backend:** Python 3.10, Flask, SQLAlchemy, Pipenv, REST APIs, JWT
- **Frontend:** JavaScript (ES6+), React.js, HTML5, CSS3, Bootstrap, Webpack
- **Databases:** PostgreSQL (Relational), Firebase / Firestore (Real-time NoSQL)

---

## ⚙️ Local Installation & Setup

### 1. Backend Setup (Python / Flask / PostgreSQL)
Make sure you have **Python 3.10**, **Pipenv**, and a running database engine (**PostgreSQL** recommended).

1. **Install Python dependencies:**
   ```bash
   pipenv install
   ```

2. **Configure environment variables:**
   ```bash
   cp .env.example .env
   ```
   Open `.env` and configure your `DATABASE_URL` according to your database engine:

   | Engine | `DATABASE_URL` Format |
   | :--- | :--- |
   | **PostgreSQL** *(Recommended)* | `postgres://username:password@localhost:5432/example` |
   | **MySQL** | `mysql://username:password@localhost:port/example` |
   | **SQLite** | `sqlite:////test.db` |

3. **Run SQLAlchemy database migrations:**
   ```bash
   pipenv run migrate
   pipenv run upgrade
   ```
   *(To revert a migration if needed: `pipenv run downgrade`)*

4. **Seed test data (Optional):**
   - Generate 5 test users via custom Flask CLI command:
     ```bash
     flask insert-test-users 5
     ```
   - Or populate full test records defined in `/src/api/commands.py`:
     ```bash
     pipenv run insert-test-data
     ```

5. **Start the Flask backend server:**
   ```bash
   pipenv run start
   ```

---

### 2. Frontend Setup (React.js)
Ensure **Node.js (v14+)** is installed and the backend server is running.

1. **Install Node packages:**
   ```bash
   npm install
   ```

2. **Start the Webpack development server:**
   ```bash
   npm run start
   ```

---

## 👥 Development Team
- **Anguibell Romero** – *Full Stack Developer (Flask REST APIs, SQLAlchemy Data Modeling & Firebase/Firestore Integration)* – [GitHub](https://github.com/Anguibell) | [LinkedIn](https://www.linkedin.com/in/anguibell-romero)
- **Andy Herrera** – *Full Stack Developer*
- **Euclides Terán** – *Full Stack Developer*
- **Guillermo Obando** – *Full Stack Developer*

---
*Built on top of the 4Geeks Academy React-Flask Full Stack architecture.*
