# Hola Mundo 1

Este proyecto es una aplicación Django sencilla creada para demostrar una configuración básica de Django con una aplicación llamada `pages` y una plantilla HTML estática.

## 📦 Estructura del proyecto

- `manage.py` - Utilidad de Django para ejecutar comandos y administrar el proyecto.
- `db.sqlite3` - Base de datos SQLite usada para desarrollo local.
- `base_project/` - Configuración principal de Django.
  - `settings.py` - Ajustes del proyecto.
  - `urls.py` - Rutas globales del proyecto.
  - `wsgi.py` / `asgi.py` - Puntos de entrada para despliegue.
- `pages/` - Aplicación Django principal del proyecto.
  - `views.py` - Vistas de la aplicación.
  - `urls.py` - Rutas de la aplicación.
  - `models.py` - Modelos de datos (actualmente vacío).
  - `tests.py` - Pruebas unitarias.
- `templates/` - Plantillas HTML del proyecto.
  - `index.html` - Página principal.

## 🧩 Dependencias

El proyecto usa Django y dependencias básicas para correr en un entorno local. Las versiones encontradas en `requirements.txt` son:

- `Django==6.0.4`
- `asgiref==3.11.1`
- `sqlparse==0.5.5`
- `tzdata==2026.2`

## 🚀 Instalación y configuración

1. Clona o descarga el proyecto.
2. Crea un entorno virtual de Python:
   ```bash
   python -m venv .venv
   ```
3. Activa el entorno virtual:
   - Windows PowerShell:
     ```powershell
     .\.venv\Scripts\Activate.ps1
     ```
   - Windows cmd:
     ```cmd
     .\.venv\Scripts\activate.bat
     ```
4. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

## 🧪 Ejecutar el proyecto

Con el entorno virtual activo, ejecuta el servidor de desarrollo:

```bash
python manage.py runserver
```

Luego abre en tu navegador:

```text
http://127.0.0.1:8000/
```

## 🎯 Qué hace el proyecto

Esta aplicación muestra una página HTML simple en la ruta raíz (`/`). Es una base ideal para:

- aprender cómo funciona Django
- estructurar un proyecto con una app `pages`
- comenzar a agregar vistas, modelos y rutas adicionales

## 📄 Archivos clave

- `templates/index.html` - plantilla HTML principal.
- `pages/views.py` - controla la presentación de la página.
- `pages/urls.py` - define las rutas propias de la app.
- `base_project/urls.py` - enlaza las URLs de la aplicación al proyecto.

## 🧠 Siguientes pasos sugeridos

- Agregar un modelo en `pages/models.py`.
- Configurar la interfaz de administración en `pages/admin.py`.
- Crear más plantillas y rutas.
- Añadir pruebas en `pages/tests.py`.

## ❗ Notas

- El proyecto usa SQLite para desarrollo, por lo que no se necesita configuración de base de datos adicional.
- Asegúrate de usar la misma versión de Python compatible con Django 6.0.4, idealmente Python 3.11 o posterior.

---

Gracias por usar este proyecto. ¡Disfruta desarrollando con Django!