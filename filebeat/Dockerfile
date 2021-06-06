FROM docker.elastic.co/beats/filebeat:7.11.1
COPY filebeat.yml /usr/share/filebeat/filebeat.yml
USER root
RUN mkdir /data
COPY logs/* /data
RUN chown root /usr/share/filebeat/filebeat.yml
RUN chown root /data
