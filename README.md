🛡️ Secure User Authentication - Django
This project is developed as part of Prodigy Infotech Internship - Task 01.
The goal is to implement a secure user authentication system with login, signup, and logout functionality in Django.
🚀 Features
✅ User Registration (Sign Up)
✅ User Login (Sign In)
✅ User Logout
✅ Secure Password Hashing (using Django’s built-in auth system)
✅ Authentication-based Route Protection (only logged-in users can access certain pages)
✅ Session Management handled by Django

🛠️ Tech Stack
Backend: Python, Django
Frontend: HTML, CSS (Django Templates)
Database: SQLite (default, can be replaced with MySQL/PostgreSQL)

📂 Project Structure
SecureAuth/
│── accounts/          # App containing authentication logic
│   ├── migrations/
│   ├── templates/     # HTML templates (login, signup, logout, home)
│   ├── views.py       # Handles user login, signup, logout
│   ├── urls.py        # Routes for authentication
│   └── models.py      # (Using Django default User model)
│
│── SecureAuth/        # Main project folder
│   ├── settings.py    # Project settings
│   ├── urls.py        # Root URL configuration
│   └── wsgi.py
│
└── manage.py          # Django management file

⚙️ Installation & Setup
Clone the Repository
git clone https://github.com/your-username/secure-auth-django.git
cd secure-auth-django

Create Virtual Environment
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows


Install Dependencies
pip install -r requirements.txt

Run Migrations
python manage.py migrate
Create Superuser (for Admin Panel)
python manage.py createsuperuser


Run Development Server
python manage.py runserver


Open in browser:
👉 http://127.0.0.1:8000/

🔐 Authentication Flow

Sign Up → User creates an account with username, email, and password.
Login → User logs in with credentials.
Session Management → Django handles authentication sessions securely.
Logout → User can log out anytime, ending the session.
Protected Routes → Certain pages (like Dashboard) are accessible only after login.

📸 Screenshots

📜 License

This project is for educational purposes as part of the Prodigy Infotech Internship.
