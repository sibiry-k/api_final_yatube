## Описание. Что это за проект, какую задачу он решает, в чём его польза.
**Yatube** — это платформа для блогов. Позволяет пользователям размещать свои статьи, комментировать их, а также подписываться на интересных авторов, объединяет людей по интересам. 

## Установка. Как развернуть проект на локальной машине.

### Клонировать репозиторий и перейти в него в командной строке:

```
git clone git@github.com:yandex-praktikum/api_final_yatube.git
```

```
cd api_final_yatube
```

### Cоздать и активировать виртуальное окружение:

```
python -m venv venv
```

```
source venv/Scripts/activate
```
### Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

### Выполнить миграции:

```
python manage.py migrate
```

## Запустить проект:

```
python3 manage.py runserver
```

## Примеры. Некоторые примеры запросов к API.

### Работа с публикациями:
Получить все публикации:
```
GET http://127.0.0.1:8000/api/v1/posts/
```
Создать публикацию:
Payload
{
  "text": "string",
  "image": "string",
  "group": 0
}
```
POST http://127.0.0.1:8000/api/v1/posts/
```
Получить JWT-токен:
Payload
{
  "username": "string",
  "password": "string"
}
```
POST http://127.0.0.1:8000/api/v1/jwt/create/
```
