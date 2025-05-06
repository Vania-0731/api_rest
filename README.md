
# Proyecto API REST de Alumno en Django

Este proyecto es una API REST simple desarrollada en Django que gestiona los datos de alumnos (nombre, apellido, correo, fecha de nacimiento, y dirección). Los usuarios pueden crear, leer, actualizar y eliminar los registros de los alumnos.

## Requisitos

Antes de comenzar, asegúrate de tener instalados los siguientes programas en tu entorno local:

- Python 3.x
- pip (gestor de paquetes de Python)
- Django 4.x
- Django REST framework

## Pasos para usar el proyecto

Sigue estos pasos para ejecutar el proyecto en tu entorno local.

### 1. Clonar el repositorio

Primero, clona este repositorio en tu máquina local:

```bash
git clone https://github.com/Vania-0731/api_rest.git
cd api_rest
```

### 2. Crear un entorno virtual (opcional pero recomendado)

Es recomendable crear un entorno virtual para mantener las dependencias del proyecto aisladas. Ejecuta lo siguiente:

```bash
python -m venv venv
```

### 3. Activar el entorno virtual

En Windows:

```bash
.
venv\Scripts\activate
```

En macOS/Linux:

```bash
source venv/bin/activate
```

### 4. Instalar dependencias

Instala las dependencias del proyecto, que se encuentran en el archivo `requirements.txt`. Si no tienes este archivo, instala las siguientes librerías manualmente:

```bash
pip install django
pip install djangorestframework
```

### 5. Configurar la base de datos

Antes de ejecutar el proyecto, necesitarás configurar la base de datos y las migraciones de Django. Ejecuta los siguientes comandos:

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Ejecutar el servidor de desarrollo

Una vez configurado el proyecto, ejecuta el servidor de desarrollo de Django:

```bash
python manage.py runserver
```

Esto iniciará el servidor en `http://127.0.0.1:8000/`. Ahora podrás acceder a la API en:

- `http://127.0.0.1:8000/api/alumnos/` para interactuar con los recursos de "Alumno" (GET, POST, PUT, DELETE).

### 7. Acceso a la administración de Django

Si deseas acceder al panel de administración de Django para gestionar los datos de los alumnos, crea un superusuario:

```bash
python manage.py createsuperuser
```

Sigue las instrucciones para crear el superusuario (nombre de usuario, correo, contraseña).

Luego, accede a la administración en:

```
http://127.0.0.1:8000/admin/
```

### 10. Finalizar

Para detener el servidor de desarrollo, presiona `Ctrl + C` en tu terminal.

