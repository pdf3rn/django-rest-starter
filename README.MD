## Django REST Starter

### Usage

Clone this repo

```bash
git clone https://github.com/pdf3rn/django-rest-starter.git
cd django-rest-starter
```

Create virtual env:

```bash
python -m venv venv
```

Install requirements

```bash
pip install -r requirements.txt
```

Makemigrations and migrate

```bash
python manage.py makemigrations
# after make migrations then migrate to DB
python manage.py migrate
```

Make superadmin account

```bash
python manage.py createsuperuser
```

Run server

```bash
python manage.py runserver
```

### All about make migrations and migrate

```bash
# show all migrations
python manage.py showmigrations
# make migrations
python manage.py makemigrations
# after make migrations then migrate to DB
python manage.py migrate
# rollback all migrations for 'app_name'
python manage.py migrate [app_name] zero
# rollback migrations
python manage.py [migrations_name] zero
``` 

### Create apps

This project has main app called 'app', you can create sub-apps under main app folder

```bash
# Create subfolder
mkdir app/app_name
# Start app
python manage.py startapp app_name app/app_name
```

Update project name in `apps.py` file adding the prefix `app.` to the app string name