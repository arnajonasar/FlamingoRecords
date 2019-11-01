FROM python:3

COPY . /app
WORKDIR /app

ENV PYTHON_ENV production

RUN pip3 install -r requirements.txt

EXPOSE 5050
CMD python ./app.py
