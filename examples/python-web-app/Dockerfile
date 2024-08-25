FROM python:3

WORKDIR /app

COPY requirements.txt /app
COPY devops /app

RUN pip install -r requirements.txt 

ENTRYPOINT ["python3"]

CMD ["manage.py", "runserver"]




