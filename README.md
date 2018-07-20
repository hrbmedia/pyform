# pyform

Best practice to use Django / Github / Virtualenv / PostgreSQL on Ubuntu

- Create repository github on github.com
- git clone ### https repository ###
- cd ### local folder ###
- if you need : install virtualenv
- create virtual env : virtualenv env
- launch virtual env : source env/bin/activate
- ignore env folder in git. create file .gitignore
- add line in .gitignore : env/ 
- pip install django
- verification : python -m django --version
- create project structure : django-admin startproject ### project name ###
- to use PostgreSQL with Django, we need library psycopg2 : pip install psycopg2
- install postgreSQL (Ubuntu includes PostgreSQL by default) : apt-get install postgresql-10
- use the operating system user postgres to create your database : sudo -u postgres -i
- enter PostgreSQL : psql
