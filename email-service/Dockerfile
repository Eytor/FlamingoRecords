FROM python

LABEL author="Mikael"

ENV PYTHON_ENV production

ADD . /email-service/

WORKDIR /email-service/

RUN pip install --no-cache-dir -r requirements.txt

CMD [ "python", "app.py" ]