# Is based on the latest ubuntu
FROM ubuntu:latest

# Update APT using apt-get update
RUN apt-get update

# Upgrade currently installed software through APT using apt-get upgrade -y
RUN apt-get upgrade -y

RUN apt-get install -y python3 python3-pip

RUN pip3 install flask

RUN pip3 install flask-cors

WORKDIR /app

COPY . /app

EXPOSE 5252

CMD ["python3", "api.py"]