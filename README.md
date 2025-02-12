Project Overview : learning_tool
================

This is a Django-based web application designed for managing learning logs. It includes basic models, views, and forms for logging learning activities. The project consists of multiple apps and configurations to handle the backend operations. This is full deployable project, I have used plaform.sh to deploy, So if your interested in deploying this project, you just need to clone this project locally and just push this project to platform.sh. For how to deploy this project you can refer to the book Eric Matthes - Python Crash Course-No Starch Press (2023). 

* * * * *

Project Structure
-----------------

The project is structured as follows:

graphql

CopyEdit

.

├── accounts                   # App for handling user accounts and authentication

│   ├── \_\_init\_\_.py             # Marks the directory as a Python package

│   ├── admin.py                # Configuration for the Django admin panel

│   ├── apps.py                 # App configuration

│   ├── migrations              # Database migrations folder

│   ├── models.py               # Defines the models for the app

│   ├── templates               # HTML templates used by this app

│   ├── tests.py                # Test cases for the app

│   ├── urls.py                 # URL routing for this app

│   └── views.py                # Views (handlers for web requests)

├── db.sqlite3                  # SQLite database file

├── learning\_logs               # App for managing learning logs

│   ├── \_\_init\_\_.py             # Marks the directory as a Python package

│   ├── admin.py                # Configuration for the Django admin panel

│   ├── apps.py                 # App configuration

│   ├── forms.py                # Forms for adding/editing logs

│   ├── migrations              # Database migrations folder

│   ├── models.py               # Defines the models for the app

│   ├── requirements.txt        # Project dependencies for this app

│   ├── templates               # HTML templates for this app

│   ├── tests.py                # Test cases for this app

│   ├── urls.py                 # URL routing for this app

│   └── views.py                # Views (handlers for web requests)

├── ll\_project                  # Main project directory

│   ├── \_\_init\_\_.py             # Marks the directory as a Python package

│   ├── asgi.py                 # ASGI configuration for asynchronous server

│   ├── settings.py             # Project settings (database, installed apps, etc.)

│   ├── urls.py                 # Main URL routing for the project

│   └── wsgi.py                 # WSGI configuration for server

├── manage.py                   # Django command-line utility for managing the project

├── project\_structure.txt       # The project structure file

└── requirements.txt            # Project dependencies

* * * * *


---

## Installation

1. Clone the repository:

    ```bash
    git clone <repository_url>
    cd <project_directory>
    ```

2. Create and activate a virtual environment:

    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows use 'env\Scripts\activate'
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Run migrations to set up the database:

    ```bash
    python manage.py migrate
    ```

5. Create a superuser to access the Django admin:

    ```bash
    python manage.py createsuperuser
    ```

6. Start the development server:

    ```bash
    python manage.py runserver
    ```

The app will be accessible at `http://127.0.0.1:8000`.

---

## Features

- **Accounts App**: Handles user registration, authentication, and user-related operations.
- **Learning Logs App**: Manages the creation, viewing, and logging of learning activities.
- **Admin Panel**: Accessible via `/admin` for managing users, logs, and other data.
- **Forms**: Provides forms to add and edit learning logs.

---

## Testing

To run the test cases:

```bash
python manage.py test




