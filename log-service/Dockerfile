FROM python

LABEL author="Mikael"

ENV PYTHON_ENV production

ADD . /log-service/

WORKDIR /log-service/

RUN pip install --no-cache-dir -r requirements.txt

CMD [ "python", "app.py" ]