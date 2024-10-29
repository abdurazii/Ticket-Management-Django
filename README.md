# Django Ticketing System

A ticketing system built using Python and Django, designed to help manage technical support requests within a company. This application supports three roles:
1. **Admin**: Assigns engineers to tickets.
2. **Customer**: Creates and tracks ticket status.
3. **Engineer**: Manages ticket resolutions.

## Features
- **Customer Role**: Register, log in, create tickets, view status (active, resolved, closed), and edit unresolved tickets.
- **Engineer Role**: View all tickets, accept and resolve tickets, and track managed tickets.
- **Admin Role**: Assign engineers to tickets through the Django admin panel.

## Getting Started

### Prerequisites
- Python 3.x
- [pip](https://pip.pypa.io/en/stable/installation/) (Python package installer)
- [virtualenv](https://virtualenv.pypa.io/en/latest/) (for creating isolated environments)

### Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/abdurazii/Ticket-Management-Django.git
    cd Ticket-Management-Django
    ```

2. **Create a virtual environment**
    ```bash
    python -m venv venv
    ```

3. **Activate the virtual environment**
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On MacOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

5. **Database Migrations**
   Run migrations to set up the database schema:

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

6. **Create a Superuser (Admin)**
   To access the Django admin interface and assign engineers:
    ```bash
    python manage.py createsuperuser
    ```

7. **Run the Development Server**
    ```bash
    python manage.py runserver
    ```

## Usage
1. **Admin**: Log in at `http://127.0.0.1:8000/admin` to assign engineers to tickets.
2. **Customers**: Register, log in, create tickets, and track ticket status.
3. **Engineers**: View and manage assigned tickets, resolve them, and track managed tickets.




---

**Note:** Remember to keep your `requirements.txt` updated if new dependencies are added.

Happy troubleshooting!
