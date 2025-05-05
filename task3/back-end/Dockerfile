FROM ubuntu:latest

FROM ubuntu:latest

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python3 python3-pip

# Supprime le marqueur d'environnement géré en externe
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install flask
RUN pip3 install flask-cors

WORKDIR /app
COPY ./api.py /app/api.py

CMD ["python3", "api.py"]
