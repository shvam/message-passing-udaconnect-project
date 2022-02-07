FROM python:3.8-buster

WORKDIR .

RUN apt-get install gcc libc-dev
COPY $PWD .
RUN pip install -r requirements.txt
EXPOSE 50050

CMD ["python", "grpc-server.py"]