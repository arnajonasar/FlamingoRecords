FROM python:3

COPY . /app
WORKDIR /app

ENV PYTHON_ENV production

RUN pip install -r requirements.txt

EXPOSE 5000
CMD python ./app.py
