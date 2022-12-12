# Portfolio Structure

Models:
- Project
- Review (unused)
- Tag

## User App
User app was created to handle users sessions, however it was no included in settings installed apps since the website is intended to just provide owner's project information to clients.

## Ips
Ips are stored as a set called ipSet and displayed with staff permissions using this URL:http://127.0.0.1:8000/ips/

## Forms (Create, Edit and delete projects)
User authentication is required to show "add project" and "logout" in the navigation bar. In addition, to delete, update or create a project the user needs staff permissions.

# Installation

Set up the virtual enviroment and clone the repository. Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the necessary libraries in an environment.

```bash
pip install -r requirements.txt
```
Then make up the .env folder with env variables in the root's parent directory (SECRET_KEY, 
DATABASE_NAME, DATABASE_USER, DATABASE_PASS, DATABASE_HOST, DATABASE_PORT, DEBUG)
Finally run the migrations and get the server started

```bash
py manage.py makemigrations
py manage.py migrate
py manage.py runserver
```

# Links
- [Template] (https://github.com/divanov11/Django-2021)
- [Matrix Effect] (https://codepen.io/wefiy/pen/WPpEwo)

