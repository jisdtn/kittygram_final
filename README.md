### Платформа c карточками кошек 

Социальная сеть для обмена фотографиями питомцев.

```commandline
Реализован backend, API, был задеплоен на сервер Яндекс.Облако в контейнерах: 
gateway, PostgreSQL и Django через docker-compose (вероятно, время аренды уже истекло).
```
### Запуск проекта в dev-режиме (только бэк):

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/jisdtn/kittygram_final
```

```
cd kittygram_final
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv venv
```

```
source venv/bin/activate
```

Установить зависимости из файла requirements.txt:

```
cd backend
```

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить backend проекта:

```
python3 manage.py runserver
```
### Примеры запросов к API.

```commandline
http://localhost/api/cats/ ('GET')
```
```commandline
http://localhost/api/cats/ ('POST')
```
```commandline
http://localhost/api/achievements/ ('GET')
```
