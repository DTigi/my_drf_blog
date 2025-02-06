# Django REST API

Этот проект представляет собой серверную часть веб-приложения, разработанную с использованием Django и Django REST Framework (DRF). Проект выложен на GitHub и предоставляет RESTful API для взаимодействия с данными.

## Технологии
- Python 3.x
- Django
- Django REST Framework
- SQLite/PostgreSQL (или другая СУБД по вашему выбору)

## Установка и запуск

### 1. Клонирование репозитория
```sh
git clone https://github.com/DTigi/my_drf_blog.git
cd your-repository
```

### 2. Создание и активация виртуального окружения
```sh
python -m venv venv
source venv/bin/activate  # для MacOS/Linux
venv\Scripts\activate  # для Windows
```

### 3. Установка зависимостей
```sh
pip install -r requirements.txt
```

### 4. Применение миграций
```sh
python manage.py migrate
```

### 5. Создание суперпользователя (по желанию)
```sh
python manage.py createsuperuser
```

### 6. Запуск сервера разработки
```sh
python manage.py runserver
```

## API эндпоинты

Приложение предоставляет RESTful API. Полный список эндпоинтов можно найти в документации Swagger или Postman (если добавлена).

Примеры эндпоинтов:
- `GET /api/posts/` — Получить список постов
- `POST /api/feedback/` — Обратная связь
- `GET /api/posts/{slug}/` — Получить информацию о конкретном посте
- `GET /api/posts/?q=` — Поиск по сайту
- `POST /api/comments/` — Добавить комментарий

## Файлы и структура проекта
```
/your-repository
│── your_project/
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   ├── asgi.py
│
│── your_app/
│   ├── models.py
│   ├── views.py
│   ├── serializers.py
│   ├── urls.py
│
│── manage.py
│── requirements.txt
│── README.md
```

## Развертывание

Для развертывания на продакшн выполните следующие шаги:

1. Настройте файл `settings.py` (отключите `DEBUG`, настройте базу данных и `ALLOWED_HOSTS`).
2. Настройте статические файлы (`collectstatic`).
3. Настройте сервер (Gunicorn, Nginx, Docker и т. д.).

## Дополнительная информация
- [Django](https://www.djangoproject.com/)
- [Django REST Framework](https://www.django-rest-framework.org/)

### Автор
**DTigi** - [GitHub Profile](https://github.com/DTigi)

