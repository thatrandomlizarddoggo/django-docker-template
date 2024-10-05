FROM python:3.8.5-alpine

RUN pip install --upgrade pip

COPY ./requirements.txt .
RUN pip install -r requirements.txt

COPY ./django_project /app

WORKDIR /app

COPY ./enterypoint.sh /
ENTRYPOINT ["sh", "/enterypoint.sh"]

