# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash:7.2.0
USER root
COPY mysql-connector-java-8.0.16.jar /usr/share/logstash/logstash-core/lib/jars/
# Add your logstash plugins setup here
RUN logstash-plugin install logstash-input-jdbc
# Example: RUN logstash-plugin install logstash-filter-json
RUN logstash-plugin install logstash-filter-aggregate
