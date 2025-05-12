# Usar una base oficial de Python
FROM python:3-slim

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar todos los archivos del build context al contenedor
COPY . /app

# Instalar las dependencias desde requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Exponer el puerto 80
EXPOSE 80

# Declarar una variable de entorno
ENV NAME=World

# Ejecutar la aplicación cuando se inicie el contenedor
CMD ["python", "app.py"]
