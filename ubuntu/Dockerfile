FROM ubuntu:14.04

ENV version 0.9
RUN hostname
RUN apt-get update && apt-get install -y python-pip python-dev libpq-dev git curl
RUN mkdir /app
WORKDIR /app

COPY *.txt /app/requirements.txt
RUN pip install -r requirements.txt

CMD ["bash"]
