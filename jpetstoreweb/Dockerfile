FROM tomcat:9.0-jre8-slim

RUN rm -rf /usr/local/tomcat/webapps/*

COPY tomcat/conf/* /usr/local/tomcat/conf/
COPY tomcat/lib/* /usr/local/tomcat/lib/

COPY ./target/jpetstore /usr/local/tomcat/webapps/jpetstore

WORKDIR /usr/local/tomcat/bin
CMD ["catalina.sh", "run"]