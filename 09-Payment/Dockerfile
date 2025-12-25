FROM python:3.9
WORKDIR /opt/server
COPY payment.ini .
COPY *.py .
COPY requirements.txt .
RUN pip3 install -r requirements.txt
# ENV are in docker compose
CMD ["uwsgi", "--ini", "payment.ini"]