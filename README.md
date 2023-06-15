# Описание сервиса
Kittygram - проект в котором пользователи могут поделиться своими котиками со всем миром. Рассказать о их шалостях и достижениях. Данный проект разделен на Backend и Frontend части. Backend построен на Django REST Framework, Frontend на REACT.

# Доступный функционал
- Управление пользователями
- Регистрация пользователей
- Публикация, удаление котиков с фото
- Просмотр котиков в ленте
- Автоматический деплой проекта в контейнерах и CI/CD с помощью GitHub Actions
- Запуск проекта происходит через Docker Container
- Отправка сообщения в Telegram Bot после завершения деплоя

# Подготовка .env файла
Для запуска проекта необходимо создать .env файл который имеет вид:
```
DEBUG=False
SECRET_KEY=<Your_some_long_string>
DNS_NAME=<Your_dns_name>
POSTGRES_DB=postgres
POSTGRES_USER=postgres
POSTGRES_PASSWORD=<Your_password>
DB_HOST=kittygram-db
DB_PORT=5432
```

# Секреты GitHub
Для автоматического деплоя необходимо запомнить секреты в проекте на GitHub:
- DOCKER_USERNAME - Username в аккаунте на DockerHub
- DOCKER_PASSWORD - Password в аккаунте на DockerHub
- USER - Логин на удалённом сервере
- HOST - IP удалённого сервера
- SSH_KEY - SSH-key компьютера, с которого будет происходить подключение к удалённому серверу
- SSH_PASSPHRASE - Если для ssh используется фраза-пароль
- TELEGRAM_TO - ID пользователя в Telegram
- TELEGRAM_TOKEN - ID бота в Telegram
