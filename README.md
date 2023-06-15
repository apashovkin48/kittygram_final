# Описание сервиса
Kittygram - проект в котором пользователи могут поделиться своими котиками со всем миром. Рассказать о их шалостях и достижениях. Данный проект разделен на Backend и Frontend части. Backend построен на Django REST Framework, Frontend на REACT.

# Доступный функционал
- Управление пользователями
- Регистрация пользователей
- Публикация, удаление котиков с фото
- Просмотр котиков в ленте
- Автоматический деплой проекта в контейнерах и CI/CD с помощью GitHub Actions
- Запуск проекта происходит через Docker Container

# Подготовка .env файла
Для запуска проекта необходимо создать .env файл который имеет вид:
```
DEBUG=False
SECRET_KEY=<Your_some_long_string>
DNS_NAME=<Your_dns_name>
POSTGRES_DB=postgres
POSTGRES_USER=postgres
POSTGRES_PASSWORD=<Your_password>
DB_HOST=foodgram-db
DB_PORT=5432
```
