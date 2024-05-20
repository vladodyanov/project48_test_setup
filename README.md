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

## GIT COMMANDS
# Stash your local changes
git stash

# Pull the changes from the remote repository
git pull origin developer

# Apply your stashed changes
git stash pop

# Клониране на хранилището (repository) локално:
git clone <URL на хранилището>
# Това ще създаде локално копие на хранилището на вашия компютър. Сега имате локална версия на отдалечените бранчове.
Тази операция се прави само първия път (Затова е стъпка 0).
Следващите стъпки описват целия процес за работа с нашето
хранилище, когато искаме да правим промени.

# 1. Преминаване към локалния 'my_branch' бранч:
git checkout my_branch -> Тази команда ви превключва към локалния 'my_branch' бранч, който отговаря на отдалечения 'developer' бранч.

# 2. Изтегляне на последните промени от отдалечения 'developer' бранч:
git pull origin developer —> Това ще синхронизира вашия локален 'my_branch' бранч с последните промени в отдалечения 'developer' бранч.

# 3. Създаване на нов локален бранч за работа:
git checkout -b my-feature —> Това ще създаде нов локален бранч с име ‘my-feature', базиран на 'my_branch', и ще ви превключи към него. Този бранч съществува само локално засега.

# 4 . Извършване на промени по кода локално:
● Редактирайте, добавяйте или изтривайте файлове според нуждите на проекта. Всички промени са само във вашия локален 'my-feature' бранч.
git status Проверете дали се намирате на 'my-feature' бранча с командата git status
● Ако не се намирате в 'my-feature', може да преминете към него с командата git checkout my-feature

# 5. Добавяне на променените файлове към staging областта локално:
git add . (за добавяне на всички променени файлове)
git add <път до файл> (за добавяне на конкретен файл)(Не задавате целия път до файла, а само пътя от текущата директория в която се намирате)
След като извършите ‘git add .’, с командата git status може да видите дали сте добавили промените, които искате, преди да продължите напред

# 6. Commit на промените локално:
git commit -m "Описание на промените" —>Това ще запази промените в локалния ви 'my-feature' бранч заедно с описателно съобщение.

# 7. Изпращане на локалния 'my-feature' бранч към отдалеченото хранилище:
git push -u origin my-feature -> Това ще създаде нов бранч 'my-feature' в отдалеченото хранилище (GitHub) и ще изпрати вашите локални промени към него. Флагът -u свързва вашия локален 'my-feature' бранч с новосъздадения отдалечен (в GitHub) 'my-feature' бранч.

# 8. Създаване на Pull Request в GitHub:
● В GitHub отворете страницата на вашето хранилище.
● Изберете вашия новосъздаден отдалечен 'my-feature' бранч.
● Натиснете бутона "New Pull Request".
● Изберете 'developer' като base бранч и вашия отдалечен
'my-feature' бранч като compare бранч.
● Попълнете заглавие и описание на Pull Request-а, описвайки
направените промени.
● Посочете хората, от които искате да получите ревю на кода.
● Натиснете "Create Pull Request".

# 9. Процес на code review:
● Посочените хора ще прегледат вашия Pull Request и ще оставят
коментари и забележки, ако има такива.
● Адресирайте коментарите, направете необходимите корекции
локално във вашия 'my-feature' бранч и ги commit-нете.
● Изпратете локалните промени към отдалеченото хранилище с git
push.
# 10.Сливане (merge) на промените в отдалечения 'developer' бранч:
● След одобрение на Pull Request-а от отговорните лица, те ще
извършат сливането на вашия отдалечен 'my-feature' бранч в
отдалечения 'developer' бранч.
# 11. Изтриване на работния бранч:
● Локално: git branch -d my-feature
● Отдалечено: git push origin --delete my-feature
   
   
   
   



