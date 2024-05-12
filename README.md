# React/DjangoRF Test Authentication App

Authentication app using React and Django REST framework with session authentication.

## Installations

* backend
```
pip install djangorestframework
pip install django-cors-headers
pip install psycopg2
pip install gunicorn
```
* frontend
```
npm install axios
npm install react-bootstrap bootstrap
```
## Backend
-> Create requirements.txt
 - python -m django --version
 - pip show psycopg2-binary
 - pip show django-cors-headers
 - pip show djangorestframework
 - pip show gunicorn
   
-> Update settings.py
 - update DB
 - update INSTALLED APPS = [
   'rest_framework',
    'corsheaders',
    'backend.user_api.apps.UserApiConfig'
   ]
   
 -> Update MIDDLEWARE = [
   'corsheaders.middleware.CorsMiddleware',
   
   
-> CREATE APPS

-> Create entrypoint.sh

## Create Dockerfile in ##FRONTEND AND ##BACKEND
## Create docker-compose.yaml in the main directory
## RUN in terminal
   - docker compose up -d db
   - docker ps -a #checks the container
   - docker-compose build
   - docker-compose up
   
   
   
   



