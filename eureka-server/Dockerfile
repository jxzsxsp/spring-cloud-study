FROM java:8
VOLUME /tmp
ADD ./target/eureka-server.jar /app.jar
RUN bash -c 'touch /app.jar'
EXPOSE 8761
ENTRYPOINT ["java","-jar","/app.jar"]