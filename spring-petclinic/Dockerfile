FROM openjdk:jre-alpine

COPY target/*.jar /opt/app.jar

ENTRYPOINT exec java $JAVA_OPTS \
           -Dserver.tomcat.accesslog.prefix=stdout \
           -Dserver.tomcat.accesslog.enabled=true \
           -jar /opt/app.jar

