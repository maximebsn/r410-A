FROM debian:11
RUN apt-get upgrade && apt-get update -y
RUN apt install -y python3-pip
RUN pip install fastapi uvicorn
WORKDIR /srv
COPY app1.py .
CMD uvicorn app1:app --host 0.0.0.0
