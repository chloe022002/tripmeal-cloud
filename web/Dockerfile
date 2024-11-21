FROM python:3.7-slim
RUN mkdir -p /app
WORKDIR /app
COPY templates /app/templates
COPY static /app/static
COPY ./requirements.txt ./dbconnect.py app.py /app/
RUN chmod -x /app/app.py
RUN pip install -r requirements.txt
ENTRYPOINT ["python","app.py"]
