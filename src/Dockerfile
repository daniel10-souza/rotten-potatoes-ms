FROM python:3.8-slim-buster

RUN python3 -m pip install --upgrade pip 

WORKDIR /app

COPY requirements.txt .

RUN python3 -m pip install -r requirements.txt

COPY . .

EXPOSE 8080

CMD ["gunicorn", "-w 3", "--bind", "0.0.0.0:8080", "app:app"]