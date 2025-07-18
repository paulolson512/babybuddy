FROM python:3.11-slim
WORKDIR /app
RUN apt-get update && apt-get install -y \
    build-essential libpq-dev curl && \
    rm -rf /var/lib/apt/lists/*
RUN pip install babybuddy
EXPOSE 8000
CMD ["babybuddy", "runserver", "0.0.0.0:8000"]
