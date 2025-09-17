# 1. Base image
FROM python:3.11-slim

# 2. Arbeitsverzeichnis im Container
WORKDIR /app

# 3. Abhängigkeiten kopieren und installieren
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# 4. gesamten Projektcode kopieren
COPY babyshop_app/ .

# 5. Expose Port
EXPOSE 8025

# 6. Environment Variable
ENV DJANGO_SETTINGS_MODULE=babyshop.settings

# 7. Startbefehl: Migration + Runserver
CMD ["sh", "-c", "python manage.py migrate && python manage.py runserver 0.0.0.0:8025"]
