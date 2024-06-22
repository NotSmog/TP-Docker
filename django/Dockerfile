FROM python:3.9-slim

WORKDIR /app

COPY requirements.in requirements.in
RUN pip install --no-cache-dir -r requirements.in

COPY . /app

CMD ["gunicorn", "project.wsgi:application", "--bind", "0.0.0.0:8000"]

