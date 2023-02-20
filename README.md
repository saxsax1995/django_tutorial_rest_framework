# This project is to practice django by using rest_framework

### This project follow by this tutorial:
`https://www.django-rest-framework.org/tutorial/quickstart/`

### For db, we can use sqlite or postgres (currently, this project based on postgres)

### First of all, you need to run this command to create environment for this project
`cd project_name`

`python3 -m venv venv`

`source venv/bin/activate`

`pip install -r requirements.txt`

### If you don't have db yet, please follow this instruction:
`sudo -i -u postgres psql`

`CREATE DATABASE django_tutorial_rest_framework;`

`CREATE USER fudo4 WITH PASSWORD 'admin123';`

`GRANT ALL PRIVILEGES ON DATABASE django_tutorial_rest_framework TO fudo4;`

### Then you need to config db info by:
### In tutorial/settings.py file, find `DATABASES` variable and setting postgresdb based on it
### After that, run this command to migrate database
`python3 manage.py migrate`

### Now, you need to create a new user:
`python3 manage.py createsuperuser`
### Run server:
`python3 manage.py runserver`
### After finished, you can go to home page `127.0.0.1/8000` to try login

### Now, you are good to go
### Other information i've comment in the code
### Try to read it to know how to use this api project