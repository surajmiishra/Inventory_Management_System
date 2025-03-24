# Inventory Management System

This is a Django-based Inventory Management System designed to manage and track inventory efficiently.

## Features
- Admin panel for managing inventory.
- User authentication and authorization.
- Database integration with SQLite (default).
- Easily deployable using WSGI or ASGI.

## Requirements
- Python 3.8 or higher
- Django 4.x or higher
- Git

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/surajmiishra/Inventory_Management_System.git
   cd Inventory_Management_System
   ```

2. **Set Up a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply Migrations**:
   ```bash
   python manage.py migrate
   ```

5. **Run the Development Server**:
   ```bash
   python manage.py runserver
   ```

6. **Access the Application**:
   Open your browser and navigate to `http://127.0.0.1:8000`.

## Deployment

1. **Collect Static Files**:
   ```bash
   python manage.py collectstatic
   ```

2. **Configure WSGI/ASGI Server**:
   Use `inventory_management/wsgi.py` or `inventory_management/asgi.py` for deployment with servers like Gunicorn, uWSGI, or Daphne.

3. **Set `DEBUG = False`**:
   Update the `DEBUG` setting in `settings.py` to `False` and configure `ALLOWED_HOSTS` with your domain or IP.

4. **Run the Server**:
   Example using Gunicorn:
   ```bash
   gunicorn inventory_management.wsgi:application --bind 0.0.0.0:8000
   ```

## Contributing
Feel free to fork the repository and submit pull requests.

## License
This project is licensed under the MIT License.

## Contact
For any inquiries, please contact [surajmiishra](https://github.com/surajmiishra).
