FROM python:3.8

WORKDIR /stocks_products

COPY /stocks_products .

RUN pip install -r requirements.txt
RUN python3 manage.py migrate
RUN python3 manage.py collectstatic

EXPOSE 8000

CMD gunicorn stocks_products.wsgi -b 0.0.0.0:8000

