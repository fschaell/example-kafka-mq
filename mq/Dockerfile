FROM ibmcom/mq:9
COPY config.mqsc /etc/mqm/
# set timezone
RUN  mv /etc/localtime /etc/localtime.bak \
    && ln -s /usr/share/zoneinfo/Europe/Berlin /etc/localtime
RUN useradd bpmw -G mqm && echo bpmw:bpmw | chpasswd