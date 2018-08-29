FROM continuumio/anaconda3:5.2.0

ENV PYTHONBUFFERED=1
ENV WEBAPP_DIR=/JSIncidentManagement

RUN mkdir $WEBAPP_DIR

WORKDIR $WEBAPP_DIR

ADD requirements.txt $WEBAPP_DIR

RUN conda install -c anaconda django=2.1 && pip install -r requirements.txt

ADD . $WEBAPP_DIR/
