
FROM --platform=linux/amd64 public.ecr.aws/docker/library/python:3.10-slim-buster as build

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5000



CMD ["python", "app.py"]

