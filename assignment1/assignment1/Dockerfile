FROM python:3.11-alpine
WORKDIR /assignment1
COPY requirements.txt .
RUN pip install -r ./requirements.txt
COPY . .
CMD ["gunicorn", "--workers", "3", "--bind", "0.0.0.0:8080", "app:app"]
