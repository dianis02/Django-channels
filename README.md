# Django-channels

Linux setup
Inside the project create the virtual environment 
```
python3 -m venv venv
```
Activate the environment
```
source venv/bin/activaten
```
Install the requirements
```
python3 -m pip install -r requirements.txt
```
Addd to the .env file the next lines
```
nano .env
```
```
DEBUG=True
SECRET_KEY=KBl3sX5kLrd2zxj-pAichjT0EZJKMS0cXzhWI7Cydqc
DATABASE_URL=sqlite:///db.sqlite3
```
Migrate the database
```
python manage.py makemigrations
python manage.py migrate
```
Run the project
```
python manage.py runserver
```
