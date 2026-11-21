# Django Lab – Part 1: Environment Setup and Project Initialization

This starter project follows Part 1 of the DTI412 Lab Assignment 3–4.

## 1. Open a terminal in the project folder

Extract the ZIP file, open the extracted `django_lab_part1` folder in VS Code, then open Terminal.

## 2. Create and activate a virtual environment (Windows PowerShell)

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

If you use Windows Command Prompt instead:

```bat
python -m venv venv
venv\Scripts\activate.bat
```

## 3. Install Django

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
python -m django --version
```

## 4. Run database migrations

```bash
python manage.py migrate
```

## 5. Start the development server

```bash
python manage.py runserver
```

Open http://127.0.0.1:8000/ in your browser.

## 6. Create an admin account (optional for Part 1)

```bash
python manage.py createsuperuser
```

Then visit http://127.0.0.1:8000/admin/.

## Project structure

```text
django_lab_part1/
├── .gitignore
├── README.md
├── requirements.txt
├── manage.py
├── training_system/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── core/
    ├── __init__.py
    ├── admin.py
    ├── apps.py
    ├── migrations/
    │   └── __init__.py
    ├── models.py
    ├── tests.py
    └── views.py
```

**Note:** This ZIP prepares Part 1 only. The database models, admin customization, sample data, ORM queries, and bonus challenges belong to later parts of the lab.
