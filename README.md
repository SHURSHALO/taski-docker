# Taski docker

Это веб-приложение, позволяющее пользователям создавать заметки.

### Клонируйте репозиторий:
git clone git@github.com:SHURSHALO/taski-docker.git

### Установите Docker и Docker Compose:
Убедитесь, что на вашем компьютере установлены Docker и Docker Compose. 
Если их у вас нет, вы можете скачать и установить их с https://www.docker.com/get-started/

### Соберите Docker-образы:
Переименуйте .env.example в просто .env или напишите собственный по примеру.

Запустите команду для сборки Docker-образов вашего проекта, предполагая, что ваш файл docker-compose.yml находится в корневой директории проекта:

docker compose up -d

Затем в выполните миграции в той же директории проекта

docker compose exec backend python manage.py migrate


### Ваши сервисы будут доступны по адресу http://localhost:8000/
