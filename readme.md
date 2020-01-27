# Django Tutorial
[Link](https://docs.djangoproject.com/en/2.2/intro/tutorial01/)

# Install Django
```
$ pip install Django
```

## Create Project
```
$django-admin startproject mysite
```

*This will make the following:*
```
mysite/
    manage.py
    mysite/
        __init__.py
        settings.py
        urls.py
        wsgi.py
```

*These files are:*

* The outer `mysite/` root directory is just a container for your project. Its name doesn’t matter to Django; you can rename it to anything you like.
* `manage.py`: A command-line utility that lets you interact with this Django project in various ways. You can read all the details about `manage.py` in `django-admin` and `manage.py`.
* The inner `mysite/` directory is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).
* `mysite/__init__.py`: An empty file that tells Python that this directory should be considered a Python package. If you’re a Python beginner, read more about packages in the official Python docs.
* `mysite/settings.py`: Settings/configuration for this Django project. Django settings will tell you all about how settings work.
* `mysite/urls.py`: The URL declarations for this Django project; a “table of contents” of your Django-powered site. You can read more about URLs in URL dispatcher.
* `mysite/wsgi.py`: An entry-point for WSGI-compatible web servers to serve your project. See How to deploy with WSGI for more details.

## Development Server
```
$ cd mysite
$ python manage.py runserver

```

You need to make sure to tap on the link to assure that Django is running accordingly.

# Creating Polls App
```
$ python manage.py startapp polls
```

That’ll create a directory polls, which is laid out like this:
```
polls/
    __init__.py
    admin.py
    apps.py
    migrations/
        __init__.py
    models.py
    tests.py
    views.py
```

This directory structure will house the poll application.
