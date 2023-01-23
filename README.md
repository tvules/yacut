# YaCut — Сократить ссылку

Проект YaCut — это сервис укорачивания ссылок.
Его назначение — ассоциировать длинную пользовательскую ссылку с короткой,
которую предлагает сам пользователь или предоставляет сервис.

## Особенности

- Генерация коротких ссылок и связь их с исходными длинными ссылками.
- Переадресация на исходный адрес при обращении к коротким ссылкам.
- REST API

## Технологии

- [Python 3.7+](https://www.python.org)
- [Flask](https://flask.palletsprojects.com)
- [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com)
- [Flask-Migrate](https://flask-migrate.readthedocs.io)

## Инструкция

**1. Клонируйте репозиторий**

```shell
git clone https://github.com/tvules/yacut.git && cd yacut
```

**2. Установите зависимости проекта**

```shell
pip install -r requirements.txt
```

**3. В корне проекта создайте `.env` файл**

```shell
FLASK_APP=yacut
FLASK_DEBUG=0
DATABASE_URI=<URI базы данных, по умолчанию "sqlite:///db.sqlite3">
SECRET_KEY=<секретный ключ>
```

*Секретный ключ можно сгенерировать [тут](https://djecrety.ir/)

**4. Запустите dev-сервер**

```shell
flask run
```

<h5 align="center">Автор проекта: <a href="https://github.com/tvules">Ilya Petrukhin</a></h5>
