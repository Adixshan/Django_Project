# Django Authentication Application

This is a Django-based web application that provides user authentication functionality, including login, signup, forgot password, change password, dashboard, and profile pages. The application uses Django's built-in authentication system and forms for user management.

---

## Features

1. **User Authentication**:
   - Login with username/email and password.
   - Sign up with username, email, and password.
   - Forgot password functionality with email reset instructions.
   - Change password for authenticated users.

2. **Pages**:
   - **Login Page**: Allows users to log in with their credentials.
   - **Signup Page**: Allows new users to create an account.
   - **Forgot Password Page**: Allows users to request a password reset.
   - **Dashboard Page**: Displays a greeting message and links to the profile and change password pages.
   - **Profile Page**: Displays user information such as username, email, date joined, and last login.
   - **Change Password Page**: Allows authenticated users to change their password.

3. **Styling**:
   - Modern and responsive design using a color palette of black, grey, white, and red.
   - Card layouts with shadow effects for a clean and professional look.

---

## Setup Instructions

### Prerequisites
- Python 3.x
- Django 4.x
- A working email configuration for password reset functionality (optional).

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
Create a Virtual Environment:

bash
Copy
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install Dependencies:

bash
Copy
pip install django
Run Migrations:

bash
Copy
python manage.py migrate
Create a Superuser (Optional):

bash
Copy
python manage.py createsuperuser
Run the Development Server:

bash
Copy
python manage.py runserver
Access the Application:
Open your browser and navigate to http://127.0.0.1:8000/.

Project Structure
Copy
myauthproject/
├── accounts/
│   ├── migrations/
│   ├── templates/
│   │   └── accounts/
│   │       ├── login.html
│   │       ├── signup.html
│   │       ├── forgot_password.html
│   │       ├── dashboard.html
│   │       ├── profile.html
│   │       └── change_password.html
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── myauthproject/
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
├── manage.py
└── README.md
Implementation Details
Key Files
accounts/views.py:

Contains the logic for handling user authentication and rendering templates.

accounts/urls.py:

Defines the URL patterns for the application.

Templates:

Located in accounts/templates/accounts/.

Each page (login, signup, dashboard, etc.) has a corresponding HTML template with modern styling.

Styling:

Inline CSS is used in each template for simplicity.

The color palette includes black (#333), grey (#f4f4f4), white (#ffffff), and red (#ff4d4d).
