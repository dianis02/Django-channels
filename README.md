# Django-channels

Inside the project create the virtual environment \
Linux command\
```
python3 -m venv venv
```
Windows command\
```
py -3.10 -m venv .venv
```
Activate the environment\
Linux command\
```
source venv/bin/activate
```
Windows command\
```
.venv\Scripts\activate
```
Install the requirements
```
python3 -m pip install -r requirements.txt
```
Addd to the .env file the next lines, or create the file if it does not exits
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
Enable a channel layer
```
docker run -p 6379:6379 -d redis:5
```
Run the project
```
python manage.py runserver
```
