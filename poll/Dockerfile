FROM python

COPY static ./static

COPY templates ./templates

COPY app.py .

COPY requirements.txt .

EXPOSE 80

ENV port=80

RUN pip3 install -r requirements.txt

CMD flask run --host=0.0.0.0 --port=80