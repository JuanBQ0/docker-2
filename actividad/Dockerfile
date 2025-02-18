# Usa la imagen base de Python 3.9
FROM python:3.9

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /code

# Copia el archivo de dependencias y lo instala
COPY ./requirements.txt /code/requirements.txt
RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt

# Copia el código de la aplicación al contenedor
COPY ./app /code/app

# Comando para ejecutar la aplicación con Uvicorn
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]
