FROM python:3.8
WORKDIR /usr/local/app
COPY . .
RUN pip install -r requirements.txt && pip install gunicorn
CMD python manage.py migrate && gunicorn lib_catalog.wsgi --bind 0.0.0.0:8000
