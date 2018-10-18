FROM tiangolo/uwsgi-nginx-flask:python3.7

MAINTAINER Rajdeep Dua dua_rajdeep@yahoo.com
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
COPY . /app 
WORKDIR app
RUN pip install -r requirements.txt
ENTRYPOINT [python]
CMD [myproject.py]