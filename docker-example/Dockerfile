##########################################################
FROM python:3.6.3
##########################################################
ENV PROJECT_DIR=/opt/pytest-example \
    TERM=XTERM
RUN apt-get update
RUN apt-get install python-rdkit librdkit1 rdkit-data
RUN useradd -ms /bin/bash noodles
RUN mkdir -p $PROJECT_DIR
WORKDIR $PROJECT_DIR
#ADD ./requirements.txt $PROJECT_DIR/requirements.txt
#RUN pip3 install -r $PROJECT_DIR/requirements.txt
ADD . $PROJECT_DIR