FROM python:3.6

ADD requirements.txt /app/
WORKDIR /app

RUN pip install -r requirements.txt -v

ADD . /app

EXPOSE 8050

CMD ["gunicorn", "-b", "0.0.0.0:80", "app:app.server"]
