# Python Web Application Environment for Docker

## Note
- Python 3.7
- Django (Standard web framework)
- Nginx


# How to use

Introduce how to use run web application easier. Other case of framework will be added soon.

## requirement.txt

Module name and version write down to `requirement.txt`.  
`requirement.txt` will be used on `docker build` using `Dockerfile` for `pip install`.

## Django

The case of using Django web framework. Sample of quick run commands below.
```
django-admin startproject projectname ./app
cd app
python3 manage.py migrate
python3 manage.py runserver
```

## Flask

The case of using Flask web framework. Sample of quick run commands below.
```
cd app
touch app.py
vim app.py # -> edit code
python3 app.py
```

Example code for Flask.
```
from flask import Flask

app = Flask(__name__)

@app.route('/)
def index();
  return "Hello, World!"

if __name__ == "__main__":
  app.run()
```
