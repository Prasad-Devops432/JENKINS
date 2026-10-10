FROM python:3.11-slim

ENV PYTHONDONTWRITEBYTECODE=1 PYTHONUNBUFFERED=1

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy only the application code (tests and pipeline files are excluded by .dockerignore)
COPY app.py .

RUN useradd --create-home appuser
USER appuser

CMD ["python", "app.py"]
