FROM python:3

WORKDIR /app

COPY requirements.txt /app
COPY devops /app

RUN pip install --no-cache-dir -r requirements.txt 

COPY . .

RUN python manage.py collectstatic --noinput

EXPOSE 8000

ENTRYPOINT ["python3"]

CMD ["manage.py", "runserver"]




