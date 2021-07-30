# Starting a new Django project

```python3 -m venv env_name```

```source env/bin/activate ```
 
```env\Scripts\activate``` if on Windows

```pip install django```

```django-admin startproject project_name```

```python manage.py startapp app_name```

- If wanting to write a basic view (e.g. index.html), ensure that the path to the templates folder (e.g. project_name/app_name/templates) is within the 'DIRS' of the settings.py file. Moreover, ensure that the name of the app is listed in the INSTALLED_APPS in settings.py.



