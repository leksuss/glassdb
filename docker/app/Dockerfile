FROM python:3.7-slim

RUN apt update && apt install -y libpcre3 mime-support postgresql-client

WORKDIR /home/src

COPY requirements.txt requirements.txt

RUN pip install -r requirements.txt

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
