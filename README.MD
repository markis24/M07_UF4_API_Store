# Nombre del Proyecto

Este es un proyecto Django con PostgreSQL.

## Configuración del entorno de desarrollo

1. Clona el repositorio:

    ```bash
    git clone https://github.com/JostinCabascango/M07_UF4_API_Store.git
    cd M07_UF4_API_Store
    ```

2. Crea un entorno virtual e instala las dependencias:

    ```bash
    python -m venv env
    source env/bin/activate  # En Windows, usa `env\Scripts\activate`
    pip install -r requirements.txt
    ```

3. Configura la base de datos PostgreSQL. Asegúrate de actualizar `settings.py` con tus credenciales de la base de
   datos.

4. Ejecuta las migraciones:

    ```bash
    python manage.py migrate
    ```

5. Inicia el servidor de desarrollo:

    ```bash
    python manage.py runserver
    ```

## Flujo de trabajo de Git

1. Cada nueva característica debe estar en su propia rama. Para crear una nueva rama, usa:

    ```bash
    git checkout -b nombre-de-la-rama
    ```

2. Haz tus cambios y luego añádelos al staging area con:

    ```bash
    git add .
    ```

3. Haz commit de tus cambios:

    ```bash
    git commit -m "Descripción de los cambios"
    ```

4. Sube tu rama y los cambios a GitHub:

    ```bash
    git push origin nombre-de-la-rama
    ```

5. En GitHub, abre un pull request desde tu rama a la rama `master`.

6. Después de que el pull request sea aprobado, puedes fusionar tus cambios en `master`.

Por favor, asegúrate de mantener tu rama actualizada con `master` haciendo regularmente `git pull origin master`
mientras
trabajas en tu característica.

## Pruebas

Para ejecutar las pruebas, usa:

```bash
python manage.py test