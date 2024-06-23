# Учебный проект API для Yatube


## Стек
- Python 3.9
- Django
- Django Rest Framework
- Djoser


## Описание

API для социальной сети,  в которой можно размещать публикации с фото, комментировать записи и подписываться на других пользователей.
### Как запустить проект:

* Клонировать репозиторий и перейти в него в командной строке:

* Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

* Если у вас Linux/macOS

    ```
    source env/bin/activate
    ```

* Если у вас windows

    ```
    source env/scripts/activate
    ```
* Обновить установщик пакетов
```
python3 -m pip install --upgrade pip
```

* Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

* Выполнить миграции:

```
python3 manage.py migrate
```

* Запустить проект:

```
python3 manage.py runserver
```

### Некоторые примеры запросов из документации:

* Создание поста:
  
```
POST /api/v1/posts/
```

* Передаем следующие данные:

```
{ "text": "string", "image": "string", "group": 0 }
```

* Подписка:

```
POST /api/v1/follow/
```

* Передаем следующие данные:

```
{"following": "string"}
```

* Частичное изменение комментария:

```
PATCH /api/v1/posts/{post_id}/comments/{id}/
```

* Передаем следующие данные:

```
{"text": "string"}
```

### Для более подробного изучения проекта можно импортировать в Postman коллекцию из директрории postman_collection (README прилагается)

### Удачи!

Автор: Milkyaway13
