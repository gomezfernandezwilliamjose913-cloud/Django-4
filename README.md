# Proyecto Django

Base web en Django 5.2 LTS, con una página de inicio en español y la aplicación `core`.

## Inicio en Windows

```powershell
.\.venv\Scripts\Activate.ps1
python manage.py migrate
python manage.py runserver
```

Abre http://127.0.0.1:8000/.

Si aún no existe el entorno virtual, créalo e instala las dependencias:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

En desarrollo se usa una clave local y `DEBUG` está activado. Antes de desplegar,
define `DJANGO_SECRET_KEY`, configura `DJANGO_ALLOWED_HOSTS` y establece
`DJANGO_DEBUG=0`. No uses la clave de desarrollo en producción.

## Pruebas

```powershell
python manage.py test
```
