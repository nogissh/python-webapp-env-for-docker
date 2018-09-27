# Python Web Application Environment for Docker

## None
- Python 3.7
- Django or Flask
- Nginx


# How to use

Introduce how to use run web application easier. Other case of framework will be added soon.

## requirement.txt

Module name and version write down to `requirement.txt`.  
`requirement.txt` will be used on `docker build` using `Dockerfile` for `pip install`.

## Django

The case of using Django web framework. Sample of quick run commands below.
```
django-admin startproject mysite django-app
echo "STATIC_ROOT = './staticfiles'" >> django-app/mysite/settings.py
docker-compose build
docker-compose up -d
```


## Flask

Coming soon...