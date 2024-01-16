### Описание:

API для проекта Yatube

### Установка:

Клонировать репозиторий и перейти в него в командной строке:

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
py -m venv venv
```

```
py -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
py manage.py migrate
```

Запустить проект:

```
py manage.py runserver
```

### Примеры запросов:

```
Получить JWT-токен:

http://127.0.0.1:8000/api/v1/jwt/create/
```

```
Обновление публикации:

http://127.0.0.1:8000/api/v1/posts/{id}/

{
"text": "string",
"image": "string",
"group": 0
}
```

```
Обновление комментария:

http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/

{
"text": "string"
}
```
