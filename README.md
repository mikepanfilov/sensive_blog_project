# Блог Sensive

Blog using Django, server part.

## Running

To start the blog, you should already have Python 3 installed. Also, next to `manage.py`, there should be a database file` db.sqlite3`.

Install dependencies:

```sh
$ pip install -r requirements.txt
```

Update the database schema in the `db.sqlite3` file. If there is no such file in the directory, a new one will be created:

```sh
$ python3 manage.py migrate
```

Run the server

```sh
$ python3 manage.py runserver
```

After that, follow the link [127.0.0.1:8000 022](http://127.0.0.1:8000) and you will see the main page.

## Environment Variables

Part of the project settings is taken from environment variables. To define them, create the `.env` file next to`manage.py` and write the data into in the following format: `VARIABLE = value`.

**To run the project, these settings are not required**, the values are already set by default.

The following variables are available:

- `DEBUG` - debug mode. Put `True` to see debugging information in case of error. It is turned off by the value `False`.
- `SECRET_KEY` - secret key of the project. For example: `erofheronoirenfoernfx49389f43xf3984xf9384`.
- `STATIC_URL` - the default is "/static/". [What is STATIC_URL](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATIC_URL).
- `STATIC_ROOT` - by default it is "None", i.e. current folder. [What is STATIC_ROOT](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATIC_ROOT).
- `MEDIA_URL` - the default is "/media/". [What is MEDIA_URL](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-MEDIA_URL).
- `MEDIA_ROOT` - the default is "media". [What is MEDIA_ROOT](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-MEDIA_ROOT).

## Project Goals

The code is written for educational purposes - this is a lesson in the Python and web development course on the site [Devman](https://dvmn.org).
