FROM python:3.8
WORKDIR /app
COPY requirements.txt .
RUN python -m pip install -r requirements.txt
COPY . .
EXPOSE 8181
EXPOSE 8282
CMD ["gunicorn", "--workers=3", "--bind", "0.0.0.0", "app:app"]
