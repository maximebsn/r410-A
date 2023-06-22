FROM debian:11
RUN apt-get update && apt-get upgrade -y
RUN apt-get -y install python3-pip
RUN apt-get -y install default-libmysqlclient-dev
RUN pip install flask-mysqldb
COPY main.py main.py
COPY /templates/forms.html forms.html
CMD flask --app main.py run
