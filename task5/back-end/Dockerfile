FROM ubuntu:latest

WORKDIR /app

RUN apt-get update && apt-get install -y python3 python3-pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

RUN pip3 install flask

RUN pip3 install flask-cors

COPY api.py .

EXPOSE 5252

CMD ["python3", "api.py"]
