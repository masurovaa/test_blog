Проект представляет собой REST API для блога с постами и комментариями. Реализована аутентификация через JWT, разграничение прав, фильтрация опубликованных постов, Swagger-документация и поддержка Docker.


Возможности API

- CRUD для постов
- Комментарии к постам
- Только автор может редактировать/удалять свои посты и комментарии
- Гости могут только читать опубликованные посты
- JWT-аутентификация
- Swagger-документация
- Docker-окружение


Установка (без Docker)

1. Клонируй репозиторий:

`bash
git clone https://github.com/masurovaa/test_blog.git
cd test_blog

1.Активируйте виртуальное окружение
    python -m venv venv
    source venv/bin/activate
2.Установи зависимости
    pip install -r requerements
3.Сделай миграции и запусти сервер
    python manage.py makemigrations
    python manage.py migrate
    python manage.py runserver


Установка и запуск через Docker:
1.Убедитесь, что у вас вас установлен Docker
2.Собери и запусти контейнер:
    docker-copmose up --build