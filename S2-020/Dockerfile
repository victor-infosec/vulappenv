FROM tomcat:8.0.15-jre8
MAINTAINER 0x0keeper@gmail.com

WORKDIR /tmp

RUN set -ex \
    && rm -rf /usr/local/tomcat/webapps/* \
    && chmod a+x /usr/local/tomcat/bin/*.sh 

COPY ROOT.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080
CMD ["/usr/local/tomcat/bin/catalina.sh", "run"]
