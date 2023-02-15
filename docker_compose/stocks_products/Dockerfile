FROM python:3.8-alpine

WORKDIR /stocks_products

RUN apk add --no-cache gcc musl-dev linux-headers
COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

RUN chmod +x entrypoint.sh

RUN python3 manage.py collectstatic

ENTRYPOINT /stocks_products/entrypoint.sh

