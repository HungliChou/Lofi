FROM python:3.8

WORKDIR /app

COPY server/requirements.txt server/requirements.txt

RUN pip3 install -r server/requirements.txt

COPY . .

WORKDIR /app/server

ENV FLASK_APP=app.py

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=8888"]
