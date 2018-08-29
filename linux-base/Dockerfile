FROM python:3.6

RUN apt-get update && apt-get install wget -y

RUN wget https://repo.continuum.io/archive/Anaconda3-5.2.0-Linux-x86_64.sh

RUN bash Anaconda3-5.2.0-Linux-x86_64.sh -b -p ~/anaconda && \
    rm Anaconda3-5.2.0-Linux-x86_64.sh && \
    echo 'export PATH="~/anaconda/bin:$PATH"' >> ~/.bashrc

RUN pip install django==2.1
