# pyform

Best practice to use Django / Github / Virtualenv / PostgreSQL on Ubuntu

##### GITHUB ####

- Create repository github on github.com

- git clone ### https repository ###

##### VIRTUALENV ####

- Enter local folder
	$ cd ### local folder ###

- if you need : 
	$ install virtualenv

- create virtual env : 
	$ virtualenv env

- launch virtual env :
	$ source env/bin/activate

##### GITIGNORE ####

- ignore env folder in git. create file .gitignore

- add line in .gitignore : 
	env/ 

##### DJANGO ####

- Install Django
	$ pip install django

- verification : 
	$ python -m django --version

- create project structure : 
	$ django-admin startproject ### project name ###

##### POSTGRESQL ####

- to use PostgreSQL with Django, we need library psycopg2 : 
	$ pip install psycopg2

- install postgreSQL (Ubuntu includes PostgreSQL by default) : 
	$ apt-get install postgresql-10

- use the operating system user postgres to create your database : 
	$ sudo -u postgres -i

- enter PostgreSQL : 
	$ psql

- start server PosgreSQL : 
	$ service postgresql start

- configure PostgreSQL to start up upon server boot : 
	$ update-rc.d postgresql enable

- create db : 
	$ sudo -u postgres -i 
	$ createdb -O ### user postgresql ### ### db name ###

- verification db
	$ psql
	$ \l

- quit psql :
	$ \q

##### DJANGO > POSTGRESQL ####

- change settings database in settings.py
	$ ### Dossier Django ###/settings.py
	...

