FROM python:3.10-slim

RUN apt-get update && apt-get install -y \
    git \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /

COPY . /

RUN pip install --no-cache-dir -r requirements.txt

CMD ["python3", "/main.py"]
