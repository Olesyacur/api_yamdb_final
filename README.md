# Проект YaMDb
### ![Я](https://yastatic.net/q/logoaas/v2/Яндекс.svg?circle=black&color=000&first=white)![Практикум](https://yastatic.net/q/logoaas/v2/Практикум.svg?color=000)

Проект YaMDb собирает отзывы пользователей на произведения. 

_Благодаря этому проекту можно:_
- оставлять к произведениям текстовые отзывы 
- ставить произведению оценку
- комментировать отзывы других пользователей
- получить список всех произведений, категорий, жанров, комментариев, отзывов

***
### Технологии

API Yatube использует open-source технологии:
- [Python 3.7 ](https://www.python.org/downloads/release/python-379/)
- [Django REST framework 3.12](https://www.django-rest-framework.org/community/3.12-announcement/)
- [Simple JWT-аутентификация с реализацией через код подтверждения](https://django-rest-framework-simplejwt.readthedocs.io/en/latest/)

_Репозиторий на Github [ссылка](https://github.com/JuliaBars/api_yamdb)._
***
### Установка

- Клонируйте проект
```
git clone <ссылка>
``` 
- Установите и активируйте виртуальное окружение
- Установите зависимости из файла requirements.txt
```
pip install -r requirements.txt
``` 
- В папке с файлом manage.py выполните команду:
```
python manage.py runserver
```
### Примеры запросов и результат
```
GET http://127.0.0.1:8000/api/v1/categories/
[
    {
        "count": 3,
        "next": null,
        "previous": null,
        "results": [
            {
                "name": "Книга",
                "slug": "book"
            },
            {
                "name": "Музыка",
                "slug": "music"
            },
            {
                "name": "Фильм",
                "slug": "movie"
            }
        ]
    }
]
```
```
GET http://127.0.0.1:8000/api/v1/genres/?search=Rock
[
    {
        "count": 1,
        "next": null,
        "previous": null,
        "results": [
            {
                "name": "Rock-n-roll",
                "slug": "rock-n-roll"
            }
        ]
    }
]
```
---
### Авторы
Студенты Я.Практикум - _Олеся Чурсина,_ _Денис Костив,_ _Юлия Орлова_
