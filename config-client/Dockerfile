FROM java:8
VOLUME /tmp
ADD ./target/config-client.jar /app.jar
RUN bash -c 'touch /app.jar'
EXPOSE 6110
ENTRYPOINT ["java","-jar","/app.jar"]