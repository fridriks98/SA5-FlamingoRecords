FROM python:3
LABEL maintainer="Friðrik Snær Ómarsson"

ENV PYTHON_ENV production

COPY . /app
WORKDIR /app

RUN pip install -r requirements.txt

ENTRYPOINT [ "python", "app.py" ]
