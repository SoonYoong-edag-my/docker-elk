ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:${ELASTIC_VERSION}
USER root
# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json

#RUN curl https://jdbc.postgresql.org/download/postgresql-42.5.3.jar -o /usr/share/logstash/logstash-core/lib/jars/postgresql-jdbc.jar
COPY ./postgresql-42.5.3.jar /usr/share/logstash/logstash-core/lib/jars/postgresql-jdbc.jar

RUN chmod +x /usr/share/logstash/logstash-core/lib/jars/postgresql-jdbc.jar