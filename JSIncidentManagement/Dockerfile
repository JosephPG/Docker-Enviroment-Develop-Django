FROM python:3.5

ENV PYTHONBUFFERED=1
ENV WEBAPP_DIR=/JSIncidentManagement

RUN mkdir $WEBAPP_DIR

WORKDIR $WEBAPP_DIR

RUN wget --quiet https://repo.anaconda.com/archive/Anaconda3-5.2.0-Linux-x86_64.sh -O ~/anaconda.sh && \ /bin/bash ~/anaconda.sh

ADD requirements.txt $WEBAPP_DIR

RUN pip install -r requirements.txt
