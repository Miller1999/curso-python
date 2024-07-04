# Version
FROM python:3.10
# Directorio
WORKDIR /app
# Copiar requerimientos
COPY requirements.txt /app/requirements.txt
# Correr requerimientos
RUN pip install --no-cache-dir --upgrade -r /app/requirements.txt
# Copiar todos los archivos del entorno local
COPY . /app
# Esto mantiene en ejecucion constante
CMD ["uvicorn","main:app","--host","0.0.0.0","--port","80"]