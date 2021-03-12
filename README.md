# Lilacs_WomenKit

A project created by Team Lilacs for SheHacks 2021.


To setup virtual environment, run the following commands:
pipenv install

To activate virtual environment run:
pipenv shell

Installing django and djangorest framework:
pipenv install django
pipenv install djangorestframework
pipenv install psycopg2

Lock pipfile:
pipenv lock

Install PostgreSQL
-> Install PostgreSQL (latest version) from https://www.postgresql.org/download/

-> Setup postgres in your system according to your OS. Eg: for manjaro it would be something like this https://dev.to/tusharsadhwani/how-to-setup-postgresql-on-manjaro-linux-arch-412l

-> Create a new database in your Postgres server and name it womenkit.
            create database womenkit;
            \c womenkit

Edit Database configurations with your PostgreSQL configurations.
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'womenkit',
        'USER': 'postgres',
        'PASSWORD': '<postgres-password>',
        'HOST': '127.0.0.1',
        'PORT': '5432',
    }
}

Run the server
 Make migrations
  python manage.py makemigrations
  python manage.py migrate
  
 Run the server
  python manage.py runserver




