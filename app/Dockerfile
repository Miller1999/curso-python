# Version
FROM python:3.8
# Directorio
WORKDIR /app
# Copiar requerimientos
COPY requirements.txt /app/requirements.txt
# Correr requerimientos
RUN pip install --no-cache-dir --upgrade -r /app/requirements.txt
# Copiar todos los archivos del entorno local
COPY . /app
# Esto mantiene en ejecucion constante
CMD bash -c "while true; do sleep 1; done"