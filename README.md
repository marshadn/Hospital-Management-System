# Hospital Management System

This project is a Hospital Management System built with Python and Django. It helps manage the daily operations of a hospital, including patient appointments, staff management, and more.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features
- **Patient Management**: Add, view, and manage patient records.
- **Appointment Booking**: Schedule and manage appointments.
- **Staff Management**: Add and manage hospital staff.
- **Department Management**: Manage different hospital departments.
- **Reports**: Generate reports for various operations.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/hospital-management-system.git
    cd hospital-management-system
    ```

2. **Create a virtual environment**:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run database migrations**:
    ```bash
    python manage.py migrate
    ```

5. **Create a superuser**:
    ```bash
    python manage.py createsuperuser
    ```

6. **Run the development server**:
    ```bash
    python manage.py runserver
    ```

7. **Access the application**:
    Open your browser and go to `http://127.0.0.1:8000`.

## Usage

- **Admin Panel**: Access the Django admin panel at `http://127.0.0.1:8000/admin` to manage patients, staff, appointments, and departments.
- **Booking Appointments**: Users can book appointments through the main interface.
- **Managing Records**: Admin users can add, edit, and delete patient and staff records.

## Project Structure

```plaintext
hospital-management-system/
│
├── hospital/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
│
├── apps/
│   ├── patients/
│   │   ├── __init__.py
│   │   ├── admin.py
│   │   ├── models.py
│   │   ├── views.py
│   │   ├── urls.py
│   │   └── templates/
│   │       └── patients/
│   │           └── patient_list.html
│   ├── appointments/
│   ├── staff/
│   └── departments/
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── templates/
│   ├── base.html
│   ├── index.html
│   └── booking.html
│
├── manage.py
└── requirements.txt
