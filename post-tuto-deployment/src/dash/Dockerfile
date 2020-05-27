FROM python:3.6

ADD requirements.txt /app/
WORKDIR /app

RUN pip install -r requirements.txt -v

ADD . /app

EXPOSE 80

CMD ["gunicorn", "-b", "0.0.0.0:8050", "app:app.server"]
