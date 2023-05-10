# Yatube API 

### Описание проекта
Реализация API для социальной сети Yatube

### Требования
* Python 3.7+

### Технологии
Python 3.7
Django 2.2.19

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
https://github.com/DeLaMia/api_final_yatube
```

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

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

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```
### Примеры запросов API
#### Запросы для постов (posts)
`http://127.0.0.1:8000/api/v1/posts/`
`GET`: Получение публикаций
`POST`: Создание публикации
`GET`: Получение публикации
`PUT`: Обновление публикации
`PATCH`: Частичное обновление публикации
`DEL`: Удаление публикации

#### Запросы для коментариев(comments)
`http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/`
`GET`: Получение комментариев
`POST`: Создание комментария

#### Запросы для коментариев по id(comments)
`http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/`
`GET`: Получение комментария
`PUT`: Обновление комментария
`PATCH`: Частичное обновление комментария
`DEL`: Удаление комментария

#### Запросы для сообществ(group)
`http://127.0.0.1:8000/api/v1/groups/`
`GET`: Список сообществ

#### Получение информации о сообществе по id(group)
`http://127.0.0.1:8000/api/v1/groups/{id}/`
`GET`: Информация о сообществе

#### Возвращает все подписки пользователя, сделавшего запрос(follow)
`http://127.0.0.1:8000/api/v1/follow/`
`GET`: Подписки
`POST`: Подписка

#### Получение JWT-токена
`http://127.0.0.1:8000/api/v1/jwt/create/`
`POST`: Получить JWT-токен

#### Обновление JWT-токена
`http://127.0.0.1:8000/api/v1/jwt/refresh//`
`POST`: Обновить JWT-токен

#### Проверка JWT-токена
`http://127.0.0.1:8000/api/v1/jwt/verify/`
`POST`: Проверить JWT-токен

### Авторы
* https://github.com/DeLaMia
