# Django-projects

Portafolio web. Dos apps fueron creadas: project y user. La segunda no está en uso ya que implementa la posibilidad de crearse cuentas, logearse y cerrar sesión,
pero se desea que el acceso sea solo para el administrador. Por otro lado, la primera sí está activa.

Después de estar logeado como admin pueden agregarse proyectos nuevos, editarlos y eliminarlos.

## Deployment

Para el deploy

```bash
  py -m venv env
  activate
  pip install -r requirements.txt
  git clone <link to the repo>
```
Después de crear el archivo .env con las variables SECRET_KEY, DATABASE_NAME (utilizé postgresql), DATABASE_USER, DATABASE_PASS, DEBUG

```bash
  cd proyecto
  py manage.py makemigrations
  py manage.py migrate
  py manage.py createsuperuser
  ...
  py manage.py runserver
```





