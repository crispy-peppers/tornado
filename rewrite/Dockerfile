FROM python:3.7

EXPOSE 8888

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY requirements.txt /usr/src/app/
COPY rewrite.py $WORKDIR
RUN pip install --no-cache-dir -r requirements.txt
ENTRYPOINT ["python3", "rewrite.py"]
