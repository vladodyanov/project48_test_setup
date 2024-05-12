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
## BACKEND
1. Create requirements.txt
 - python -m django --version
 - pip show psycopg2-binary
 - pip show django-cors-headers
 - pip show djangorestframework
 - pip show gunicorn
2. Update settings.py
 - update DB
 - update INSTALLED APPS = [
   'rest_framework',
    'corsheaders',
    'backend.user_api.apps.UserApiConfig'
   ]
 - update MIDDLEWARE = [
   'corsheaders.middleware.CorsMiddleware',
   ]
3. CREATE APPS
4. Create entrypoint.sh
5. Create Dockerfile in ##FRONTEND AND ##BACKEND
6. Create docker-compose.yaml in the main directory
7. RUN in terminal
   - docker compose up -d db
   - docker ps -a #checks the container
   - docker-compose build
   - docker-compose up
   
   
   
   



