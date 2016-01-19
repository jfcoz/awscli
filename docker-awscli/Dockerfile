FROM debian
MAINTAINER jfcoz
RUN apt-get update \
  && apt-get install -y python3 wget \
  && wget https://bootstrap.pypa.io/get-pip.py \
  && python3 get-pip.py \
  && rm get-pip.py \
  && pip install aws-shell \
  && apt-get clean
ENTRYPOINT aws-shell
