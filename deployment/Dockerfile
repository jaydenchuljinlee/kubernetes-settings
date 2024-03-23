FROM python:3.12
ENV PYTHONUNBUFFERED=1
WORKDIR /server

COPY . /
RUN python3 -m venv venv
RUN ./venv/bin/pip3 install django
# RUN ./venv/bin/python3 manage.py runserver
CMD ["./venv/bin/python3", "manage.py", "runserver", "0.0.0.0:8000"]
# CMD ["ls"]

EXPOSE 8000
