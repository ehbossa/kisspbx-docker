FROM tomcat:11.0.15-jdk25-temurin-noble
MAINTAINER Iñaki Cívico "icivico@gmail.com"
WORKDIR /usr/local/tomcat/conf
RUN rm -f tomcat-users.xml context.xml
ADD tomcat-users.xml tomcat-users.xml
ADD context.xml context.xml
WORKDIR /usr/local/tomcat/webapps/
ADD https://github.com/bitinventions/kisspbx/releases/download/v0.1.1/kisspbx.war kisspbx.war
WORKDIR /usr/local/tomcat
CMD ["catalina.sh", "run"]
EXPOSE 8080
