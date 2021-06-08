ARG ELK_VERSION

FROM docker.elastic.co/beats/filebeat:${ELK_VERSION}
COPY filebeat.yml /usr/share/filebeat/filebeat.yml
USER root
RUN mkdir /data
COPY logs/* /data
RUN chmod go-w /usr/share/filebeat/filebeat.yml
RUN chown root /usr/share/filebeat/filebeat.yml
RUN chown root /data
