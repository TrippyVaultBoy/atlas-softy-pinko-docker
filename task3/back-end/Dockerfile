# Is based on the latest ubuntu
FROM ubuntu:22.04

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y python3 python3-pip python3-setuptools python3-dev build-essential

RUN pip3 install flask

RUN pip3 install flask-cors

WORKDIR /app

COPY . /app

EXPOSE 5252

CMD ["python3", "api.py"]