FROM python:3.14.0rc2-alpine3.22 AS builder

RUN apk update \
    && apk add gettext
RUN /bin/sh -c "adduser  -s /bin/sh -h /var/flask -D flask" 
WORKDIR /var/flask
USER flask
RUN python3 -m venv ~/.venv && . ~/.venv/bin/activate
COPY --chown=flask:flask . .
RUN pip install -r requirement.txt
EXPOSE 9999
ENTRYPOINT ["python3","app.py"]
