# Project setup

After cloning the repo do the following commands:

* Create a new virtual environment, then activate it.

```cmd
python -m venv venv
venv\Scripts\activate.bat
```

* Install the requirements:

```cmd
pip install -r requirements.txt
```

* Init the application, for linux:

```cmd
set FLASK_APP=app.py
set FLASK_DEBUG=true
```

* Create and init the database migration tool, must be done if you want to create the database for the first time.

```cmd
flask db init
flask db migrate
flask db upgrade
```

* Run the application

```cmd
flask run
```