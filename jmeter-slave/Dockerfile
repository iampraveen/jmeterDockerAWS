FROM praveenics/testrepo:jmeterbase
MAINTAINER Praveen

# Expose ports for JMeter Slave
EXPOSE 1099 50000
COPY entrypoint-slave/entrypoint.sh /
RUN chmod +x .entrypoint-slave/entrypoint.sh

# Run command to allocate the default system resources to JMeter at 'docker run' and start jmeter-server with all required parameters
ENTRYPOINT ["entrypoint-slave/entrypoint.sh"]
