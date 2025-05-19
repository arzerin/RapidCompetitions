# django-app/Dockerfile

FROM python:3.11-slim

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /app

COPY requirements.txt /app/
RUN pip install --upgrade pip && pip install -r requirements.txt

COPY . /app/

# Default CMD to run Django server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]