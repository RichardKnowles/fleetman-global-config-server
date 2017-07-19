FROM openjdk:8u131-jre

MAINTAINER Richard Knowles "richard@inceptiontraining.co.uk"

RUN wget -O activemq.tar.gz http://archive.apache.org/dist/activemq/5.14.3/apache-activemq-5.14.3-bin.tar.gz


# I think we can use ADD to get this for free?
RUN tar -xzf activemq.tar.gz

# Entrypoint can't be overridden at container start....
CMD ["apache-activemq-5.14.3/bin/activemq", "console"]
