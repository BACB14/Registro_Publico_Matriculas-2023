# Registro Público de Matrículas 2024

Esta aplicación web proporcionará un **Registro Público de Matrículas** para el año 2024, utilizando FastAPI como framework para la API y MySQL como base de datos para almacenar la información de las matrículas.

<image src="https://res.cloudinary.com/rodpoblete/image/upload/v1697132889/fast-api.drawio_afnvze.png" alt="Arquitectura de la aplicación" caption="Arquitectura general de la aplicación">

## 📄Requisitos

- Python 3.x
- FastAPI
- MySQL Server
- MySQL Client (p. ej., `mysql-connector-python`)
- Otros requisitos especificados en `requirements.txt`

## ⚒️Instalación

1. Clona el repositorio desde GitHub:

```bash
git clone https://github.com/tuusuario/registro-matriculas-2024.git
cd registro-matriculas-2024
```

2. Crea y activa un entorno virtual (opcional pero recomendado):

```bash
python3 -m venv venv
source venv/bin/activate  # En Windows, use: venv\Scripts\activate
```

3. Instala las dependencias desde el archivo `requirements.txt`:

```bash
pip install -r requirements.txt
```

4. Configura la base de datos MySQL editando el archivo `config.py` y agregando las credenciales adecuadas:

```python
MYSQL_USER = 'tu_usuario'
MYSQL_PASSWORD = 'tu_contraseña'
MYSQL_HOST = 'localhost'
MYSQL_DB = 'registro_matriculas'
```

5. Inicia la aplicación:

```bash
uvicorn main:app --reload
```

La aplicación estará disponible en `http://localhost:8000`.

## 💻Uso

La API permite realizar operaciones CRUD (Crear, Leer, Actualizar y Eliminar) para gestionar las matrículas. Puedes acceder a la documentación de la API en `http://localhost:8000/docs` para obtener más detalles sobre cómo utilizarla.

## 🤝Contribución

Si deseas contribuir a este proyecto, por favor sigue estos pasos:

1. Crea un fork del proyecto.
2. Crea una rama con un nombre descriptivo: `git checkout -b feature/nueva-funcionalidad`.
3. Realiza tus cambios y asegúrate de que las pruebas pasen.
4. Realiza un commit con un mensaje descriptivo: `git commit -m "Agregada nueva funcionalidad"`.
5. Sube tus cambios a tu repositorio: `git push origin feature/nueva-funcionalidad`.
6. Crea un pull request en GitHub.

## 🔎Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE.md) para más detalles.
