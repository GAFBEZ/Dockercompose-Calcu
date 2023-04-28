FROM python:3.7-alpine

WORKDIR /app

COPY . .

RUN pip install -r requirements.txt

EXPOSE 5000

#CMD ["python3" , "app.py"]

CMD ["gunicorn", "--bind", "0.0.0.0:5000", "wsgi:app"]



