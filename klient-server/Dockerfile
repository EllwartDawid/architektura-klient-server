FROM python:3.8

WORKDIR /app

COPY requirements.txt /app/
RUN pip install -r requirements.txt
RUN pip install gunicorn psycopg2

COPY . /app/

EXPOSE 8080
ENTRYPOINT ["/bin/sh"]
CMD ["run.sh"]
CMD [ "python", "create_admin.py"]
