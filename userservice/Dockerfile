# userservice/Dockerfile
FROM python:3.11-slim

# Setze das Arbeitsverzeichnis
WORKDIR /app

# Kopiere Code & Abhängigkeiten
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

# Starte die App mit uvicorn
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8111"]
