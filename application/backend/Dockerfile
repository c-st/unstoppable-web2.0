  
FROM tiangolo/uvicorn-gunicorn-fastapi:python3.8

WORKDIR /app

RUN apt update && \
    apt install -y postgresql-client zip

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .
