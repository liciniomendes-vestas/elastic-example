ARG ELK_VERSION

FROM docker.elastic.co/beats/metricbeat:${ELK_VERSION}
COPY metricbeat.yml /usr/share/metricbeat/metricbeat.yml
USER root
RUN chmod go-w /usr/share/metricbeat/metricbeat.yml
RUN chown root /usr/share/metricbeat/metricbeat.yml
