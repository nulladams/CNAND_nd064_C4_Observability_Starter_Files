FROM alpine:3.8

RUN apk add --no-cache py3-pip python3 && \
    pip3 install flask requests

COPY . /usr/src/fronttest

ENV FLASK_APP fronttest.py

WORKDIR /usr/src/fronttest

CMD flask run --host=0.0.0.0 --port=8050